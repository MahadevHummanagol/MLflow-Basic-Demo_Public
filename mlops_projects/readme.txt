python -m venv mlopSenv. --> create environment 
source mlopSenv/bin/activate --> activate environment 

deactivate --> deactivate environment

<--------Git------>
#Go to your project folder
            cd /path/to/your/project

# Initialize Git
            git init

 # if your folder was not uploading properly:   
            git rm --cached mlops_projects
            rm -rf mlops_projects/.git  

# Create .gitignore
            touch .gitignore

# Add files
            git add .

 #   Commit
 git commit -m "initial clean commit"        

# Connect to GitHub repo
        git remote add origin https://github.com/MahadevHummanagol/MLflow-Basic-Demo_Public.git

# Set branch

        git branch -M main

# Pull (IMPORTANT ⚠️)
👉 Because repo already had files:

            git pull origin main --allow-unrelated-histories --no-rebase
            ✔ This merges local + GitHub code

# git push -u origin main
            git push -u origin main


<----- IF FILES NOT VISIBLE (THIS WAS YOUR CASE) ------>

 #Remove hidden git inside folder
            git rm --cached mlops_projects
            rm -rf mlops_projects/.git

#Add files properly
            git add mlops_projects
            

# commit
            git commit -m "fix: added actual project files"

# push

            git push




