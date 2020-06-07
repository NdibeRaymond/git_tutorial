We are going to implement a manual version control work-flow, and then, try to imitate
it with git to help you understand the purpose of git.

## Steps

**Creating our first branch**
  create a folder and name it master
  inside the master folder, create a file named "cv.txt"
  open cv.txt and write the following:
  "Hello git world!, This is my cv"
  save cv.txt


**Creating our second branch**
  inside master, create a second folder named "cv_and_cover-letter" and open the new folder
  copy cv.txt from master into the new folder
  create a new document in the new folder and name it "cover_letter.txt"
  open cover_letter.txt and type the following then save:
  "Hello git world again!, This is my cover letter"
  after saving cover_letter.txt, open cv.txt in cv_and_cover-letter folder and add:
  "git is for everybody"
   save the document cv.txt


**Merge cv_and_cover-letter into master**
  open cv.txt in the master folder and add the following:
  "git is fun!"
  save the changes made to cv.txt
  copy the contents of cv_and_cover-letter folder and paste them into master
 
  oopss!, you get a prompt asking for further information (this a crude approximation of a merge conflict in git)
  the prompt occured in this case because we have cv.txt in both folders. (note that this is not exactly the 
  way it works in git. this is because git will compare the content of the cv.txt file in both branches and
  only throw a merge conflict error if the two files have changed. if cv.txt was changed only in one branch,
  then it just combines the two files)
  In windows, the prompt thrown will ask you to either "copy and replace", "don't copy" or "copy and keep both files".
  we will be choosing "copy and keep both files" since any of the other options will make us lose changes
  made to either of the file in both folders.
  After selecting "copy and keep both files" we now have two files named "cv.txt" and "cv (2).txt" in the master folder.
  open "cv (2).txt", copy the difference between the file and that of master (the difference is the line that says "git is for everybody") and paste the difference into cv.txt. now we can delete "cv (2).txt"
  because cv.txt now contains everything in "cv (2).txt"
  
congrats!, you just fixed a merge conflict (crude approximation of it anyway), and successfully merged 
cv_and_cover-letter into master. if you followed the instructions step by step, your solution should be the same with the content of "solution" folder.
next, we will be implementing what we just did with git

for more detailed explanation and to learn how to make your first [open-source](https://open-source) contribution by adding your name to the first-contributions.md file, consider checking out this [blog post](https://ndiberaymond.pythonanywhere.com/dksldks/)