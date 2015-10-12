Each of you should add a reflection file to the same repo. Be sure to start on a feature branch! Create a new file named Lastname-reflection.md. Answer the following questions in that file using Markdown. Go through the git workflow to add, commit, make a pull request, and merge it to the master repo.

Answer these questions in your reflection:

1. What git concepts were you struggling with prior to the GPS session?

  - Prior to the GPS, I was struggling with remembering to frequently `git add` and `git commit`.  Because of that, my `git commit -m`s were really long because I made a lot of changes.  Also, I was not sure when to delete the branches in the local repository (should it be done before or after the pull request gets approved & merged.)

2. What concepts were clarified during the GPS?

  - During the GPS, the guide answered our questions about what to look out for in code reviews of pull requests.  He also answered my questions about what are the best practices, and how do people actually approve/merge pull requests in a real work environment if there is a conflict (does the person who made the pull request sit with the approver while)

   Also `git clone` is the first time that a repo is `git pull`-ed to a local machine.  And `git pull` is essentially `git fetch` and `git merge` combined automatically.  Some people prefer to use `git fetch` and `git merge` separately so that they can see/inspect the changes that have happened before merging with the code in the local machine's repo.

   We did the "Release 5: Merge Conflict" after the guide needed to leave, but we were able to replicate the error message that appeared.  In the beginning, we (my pair and I) thought that the error message would appear on the command line, but it actually appears inside the file itself.  

   Also, this merge conflict does not happen if 2 people do `git pull` and `git push` their own branches at the exact same second even when their branch names are exactly the same, just because of the way that data packets get sent through networks (the milliseconds make a huge difference!).  This would just cause 2 pull requests to appear.  

   The merge conflict will happen if 1 person who does a `git add`, `git commit`, & `git push` makes a change both in the master branch and the feature branch, and does not merge them first.  But it's really easy to fix the error in git because the error message says exactly where the conflict is.  

3. What questions did you ask your pair and the guide?

 - I asked the guide the questions that I was confused about in #1 & #2.  

4. What still confuses you about git?

  - I forgot to ask this during our GPS, but I should have asked is it possible to merge something that was `git fork`-ed back to the original, aside from only merging branches within the same repo.  

   Also, I asked the guide about the difference between `git merge` & `git rebase`, but he said that this difference is not something that we need to deal with at this point.  

5. How was your first experience of pairing in a GPS?

  - On my first attempt at pairing with a GPS, I kept getting kicked out of Google Hangouts, so I was not able to do it.  I didn't really like that, because it was frustrating and annoying since before the actual Google Hangout event, I tested all my equipment and connection and it was fine.  

   So I had to switch computers to my desktop instead of my laptop, since it has more powerful hardware.  I did this, because I wanted to make sure that nothing else will go wrong again.  (Originally, my dev environment was in my laptop, because that makes it easier for me to) 

   During the actual GPS that connected successfully, our GPS guide person had some weird error in his calendar, so he thought it actually started at 9:30 am instead of 9:00 am.  But because of everything else that happened, that wasn't so bad in comparison, and it's an honest mistake.  

   The actual experience itself was not intimidating at all, and I liked it because the we were able to ask the guide some questions, and in the end, I asked him for feedback and best practices for anything git-related.  So based on this experience it seems that the guide is more of someone who observes and reports, and only gives answers if asked.  Being in charge of keeping time also falls on the pair programmers.  I think this is something to remember for next time.  

   The only negative thing that I thought about the GPS (and it's not that bad), is that the wording is a little ambiguous about who will do what.  As the navigator, when I was reading the instructions in "Release 5: Merge Conflict":
   "
    1. The driver should create a branch called small-conflict, make any change in awesome_page.md, add and commit.
    2. Check out the master branch. In the same place that you made a change on awesome_page on the branch small-conflict, make a different change. Add and commit this change.
    3. Merge the small-conflict branch to the master. Discuss what you are doing when you merge two branches together like this. 
   "
   It was not clear if #2 was for the navigator to do, and #3 is for both the navigator & driver to do; instead of all 3 should be done by the driver only.  
   We were able to figure out which one to do only because we were not getting the expected error message.