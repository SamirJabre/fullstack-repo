So basically the first thing to do is : 
1) *Make a fullstack repo in github with README file , clone it into desktop,
   *Make a frontend repo in github
   *Make a backend repo in github

2) Second thing is to add both repos (frontend and backend ) as a submodules in the fullstack repo by : git submodule add (repo link)

3) And then create a config.yaml file for configration variables

4) And then create a python file that read the configration (config_reader) from the fullstack repo 

5) Create a main python file to find the config reader and load them

6) After adding and commiting and pushing on all repos , we make sure that it work by trying to clone our main repo (fullstack-repo) into our desktop by 
   git clone --recurse-submodules (fullstack-repo link)
   this command line is to clone the whole repo with the 2 repos inside it (frontend , backend)
   


   So the last architecture of the fullstack-repo will be as follow :

   .git
   backend-repo
   frontend-repo
   .gitmodules
   config.yaml
   config_reader.py
   README.md

   Also there is a graph image showing the whole architecture of the proccess is the github repo