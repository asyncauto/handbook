
## Why is code review important?  
helps catch developer blindspots
find design pattern flaws
find obvious security issues

## How to submit a code for review?
Create a task with these info in description:
- Merge request
- Solution document link
- A screen recording of how the feature works
    - can use Loom for recording the screen. Ex: https://www.loom.com/share/41c3808152d54428bfab72d714a407d4
- An environment where the features can be tested
    - In wishup's case, this can be app-dev.wishup.co itself
    - How to deploy feature branch to app-dev
        - checkout the git branch you want to deploy
        - run 'eb deploy cb-dev' in terminal
        - if it fails at npm install, add .ebignore with the same content as .gitignore in the root directory and try again
