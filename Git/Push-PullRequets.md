# GIT: PUSH - PULL REQUESTS

##  === STEPS TO PUSH SOURCE CODE FROM PC TO GITHUB SERVER ===
1. Create a new repository to GitHub

          $ git init  
   
2. Create a new repo in PC
   
          $ git add <filename>  
   
3. Add all file in current folder

          $ git add .  
        
- Add all folder and file in <foldername>.

          $ git add <foldername>  
          $ git add <foldername>/*  
        
4. Push your code to the Staging Area

          $ git commit -m "...commit something..."  
   
5. Push your code to the Local repo
   
          $ git remote add origin <URL: https:SSH>  
   - Operation: You have a repo which name origin, URL: ...

6. Push your code to the GitHub server with address: URL...
   
          $ git push -u origin master 
   
   - <brand: master> : Push your code to branch master in server.
   - ... origin <differentBranch> : push to a different branch.
   + Operation: Push to repo on server in branch master
     Example:         Someone edit your code on GitHUb repository

### === To sync changes in GitHub to your PC ==
       
         $ git pull 

But someone edited your code, and you didn't sync to your PC. 
You edit your code on your PC, then your SYNC: 
        
         $ git push 
        
** !!! CONFLICT !!! **

- Solution: 

         $ git pull 
        
After that, we have 2 choices: use the current code | use the changed code on GitHub repo.
        I choice the first choise!
        
                $ git add .
                $ git commit -m "..."
                $ git push

 ... ok!
## === CLONE: GET SOURCE FROM GITHUB ===
** To CLONE(download) a PUBLIC source from GitHub **
        - You use: 
        
         $ git clone <URL> 
        
Example: You download Project source code. In terminal, you are sitting at: 

         ~/Documents/Project$ ...git clone <URL> 
                
All source code will be downloaded to this dir: Project
1. See the current remote URL

         $ git remote -v 
   
- Example: In my PC, at path ~/Documents/Programming_Pri
   
        $ git remote -v
     
I get:
     
        `origin  https://github.com/doduyquy/Programming_Pri.git (fetch)`
        
        `origin  https://github.com/doduyquy/Programming_Pri.git (push)`        
        
3. Update the remove URL with git remote set-url using the current and new remote URLs:

        $ git remote set-url origin <URL>

### =======================OK=======================
     




        
