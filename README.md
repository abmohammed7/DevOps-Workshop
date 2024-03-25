# DevOps-Workshop

**Create a new directory to store all the github code**
Open your favorite text editor for example VS code. Go to terminal and type the following Command
   mkdir DevOpsWorkshop #Creates DevOpsWorkshop directory
   cd DevOpsWorkshop #change directory to DevOpsWorkshop

**Clone the github repository using below command from your terminal (VS code)-**
   git clone https://github.com/abmohammed7/DevOps-Workshop.git
   cd DevOps-Workshop #change directory 

**Let's create first workflow file -**
**Method 1 -**
1. Open DevOps-Workshop folder ==> From VS code click on file> open folder > folder name
2. Click new file and create a workflow file under .github/workflows. File name should be unique please use the naming convention: Lastname-workflow.yaml

**Method 2 -**
1. Go to terminal and enter below commands
2. cd .github/workflows/
3. touch yourlastname-workflow.yaml #please makesure you change your lastname here

**Let's add some code to workflow **
1. Open the above file to create our first workflow and add below code
``` yaml   
name: Lastname-workflow #makesure to change the lastname here
on: [push]

jobs:
  run-shell-commands:
    runs-on: ubuntu-latest
    steps:
      - name: echo something
        run: echo "Hello Deloitte DevOps Aspirants"
      - name: Multiline Commands
        run: |
          node -v
          npm -v

**Save the file and push the code to the respository using below commands**
1. git add -A
2. git commit -m "Lastname workflow"
3. git push -u origin main
