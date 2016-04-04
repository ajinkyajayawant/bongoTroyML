# bongoTroyML
### git basic commmands:
```bash
cd c/Users/alokdiwakar/Documents/MachineLearning/BongoTroy
git init 
git add .
git commit -m "Adding new files"
git remote add troy https://github.com/alok7/bongoTroyML.git
git push troy master
```

# Running code on sharada
### Logging in
Remote server run script, -X is for ssh view graphics, replace ajinkyajayawant by username
`ssh -X ajinkyajayawant@sharada.ee.iitb.ac.in`
### Copying
(Syncing) files from local directory to sharada, -r option is for recursive, ./* means all files in the current directory, ~/ is the home directory of your sharada account
`rsync -r ./* ajinkyajayawant@sharada.ee.iitb.ac.in:~/`
(Syncing) files from sharada to local directory, -r option is for recursive, ./* means all files in the current directory, ~/ is the home directory of your sharada account
`rsync -r ajinkyajayawant@sharada.ee.iitb.ac.in:~/* ./`
For only copying a single file -r option is not needed
`rsync ajinkyajayawant@sharada.ee.iitb.ac.in:~/svm_try.py ./`
