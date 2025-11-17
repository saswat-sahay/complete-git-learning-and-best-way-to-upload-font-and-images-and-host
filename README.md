### In the first commit we directly pushed the images and fonts to github that is not the best way

### we have to convert the font into woff2 format because it is very light-weight font

### we have to convert the images.jpeg to webp


### now lets this site with the help of github
steps:
1. click on the settings, check reference from step 1.png image
2. click on the pages, check reference from step 2.png image
3. change the branch from none to main and save, check reference from step 3.png image
4. wait for some time to host it and just enjoy
5. change your project and it will reflect in your published website within minutes
6. if you're not able to see the changes do the hard reload (ctrl + shift + r)

### How to Back track in your project

git reset --hard HEAD~number of itereation you want to go back

e.g. if you want to go back one step
git reset --hard HEAD~1

e.g. if you want to go back two step
git reset --hard HEAD~2

### Branching
git branch branch name - to create branch
git switch branch name - to move around branches

Main branch me Maine ek branch.txt file banaya tha, jisme maine sirf ek line likha tha
NewBranch me maine do line ka code likha tha
aur sb ko commit krne ke baad
jb hm main branch me aate h to hame ek line ka code dikhta hai aur jb hm newbranch me aate h to hame 2 line ka code dikhta hai

### merge
* come to main branch
git merge branchname

### Handling conflict in merging

jb bhi main aur newbranch me same line me alag alag code hota h to conflict aata h ki kon sa change ko add kre
e.g - agar main branch ke line 3 me "hello" liikha h aur new branch me "hey" likha hua h to fir conflict aayega ki hello ko add kre ya hey ko add kre ya dono ko add kre

these are the options given by git
Accept Current Change, Acceot Incoming Change, Accept Both Changes, Compare Changes

### deleting branch
git branch -d branchName

### stashing

jb bhi aap kisi branch me kuch code likhte ho aur bina add,commit kiye hue brancg change krete ho to git aapko wo krne se rokta h, qki git wo codes delete ho jaayega branch switch krne se (qki add commit nhi kiya gya)

agar aap codes ko rakhna to caahte ho pr add commmit nhi krna caahte aur saath me hi aapko kisi aur branch me kisi kaam se jaana ho to aap apne changes/codes ko draft kr skte ho

draft krne se wo changes/codes add commit nhi honge pr delete bhi nhi honge
aur issi ko bolte h stashing

codes:
git stash
git stash apply

### deleting draft
git stash clear
