## Git branching dilemmas..


### What kinds of branch I can create?
**master:** anything that goes to production goes via master
**develop:** contains code for what ever its there master + new feature that will go next.
**feature/{feature_name}:** a new feature that I am working on. I will create the branch from develop.
**hotfix/{bug_name}:** I encountered a bug in production. I will create the branch from master.  

### I am done with a feature development in feature/{name}. What shall i do now?
Once i am done with the feature testing I will merge the branch to develop. I will merge to develop when I am 100% sure that feature will go next to production. Else I will park the feature for a while.

### I have merged my feature branch into develop, but i encountered a bug while testing in develop?
I will solve the bug in the develop branch itself. I won't create a new branch for the bug fix if the code is not in master/production.

###  Can I create multiple feature branches? 

Yes. If I am working on a feature that got deprioritized and want to work on a new feature, I will park the feature and will create a new feature/{new_feature} branch from develop branch.  

### Production system encountered a bug, How shall I push the fix? 
I will create a branch hotfix/{name} from master. Fix the bug. Merge one copy to master and one copy to develop.

