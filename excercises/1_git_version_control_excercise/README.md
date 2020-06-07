 
## Steps

### Download and install Git
* https://git-scm.com/downloads

### Create a folder and open command line
 * create a new folder (make sure this folder is outside the cloned git repository containing this "README.md" file)
 * confirm the successful installation of git by running the following command on your command line
learn more about the command line [here](https://tutorial.djangogirls.org/en/intro_to_command_line/)
```bash
    git --version
```

Initialize an empty git repository
 * run the following command to initialize a empty git repo
```bash
    git init
```
 * a ".git" folder should appear inside your folder. If you don't see any .git folder, it might be that you 
didn't enable "show hidden folders" on my local machine. you can learn how to do that [here](https://www.howtogeek.com/194671/how-to-hide-files-and-folders-on-every-operating-system/).
if you don't want to permanently make hidden folders visible, just run the command:
```bash
    dir /A
```
for windows and the command:
```bash
    ls -a
```
for linux to comfirm that the .git directory exists. you can learn more about the command line [here](https://tutorial.djangogirls.org/en/intro_to_command_line/)

### Create your cv and commit to git
 * create a new text document with the name "cv.txt" and type these words inside "Hello git world!, this is my cv".
 * then run the following command to commit it to git:
```bash
    git add .
    git commit -m "committed cv.txt to master branch"
```
Congrats!! you just created your first git commit!!. lets continue

### Cover letter branch
 * create a new branch named "cv_and_cover-letter" and switch to it like so:
```bash
    git branch cv_and_cover-letter
    git checkout cv_and_cover-letter
```
 * create text document "cover_letter.txt" and add the following words to it: "Hello git world again!, this is my cover letter"
 * save your document
 * open cv.txt and add the following to it: "git is for everybody"
 * save your document, add latest changes to git and commit it like so:
```bash
    git add .
    git commit -m "committed cover_letter.txt to cv_and_cover-letter branch and made changes to cv.txt"
```

### Make Changes to cv.txt in master
 * switch to master branch
```bash
    git checkout master
```
 * open cv.txt and add the following to it: "git is fun!"
 * save cv.txt and run the following git command to commit the changes:
```bash
  git add .
  git commit -m "modified cv.txt"
```

### Merge cv_and_cover-letter branch into master
 * run the following command:
```bash
    git merge cv_and_cover-letter
```
oopss!, a merge conflict!

don't worry, it can be fixed. The merge conflict occured because we made changes 
to cv.txt in both master and cv_and_cover-letter branches. to fix it,
 * open cv.txt
 the file should look like this:

```bash
Hello git world!, this is my cv
<<<<<<< HEAD
git is fun!
=======
git is for everybody
>>>>>>> cv_and_cover-letter
```

 * to fix the conflict, remove every thing you wouldn't like to be in the file, like
"<<<<<<< HEAD","=======", ">>>>>>> cv_and_cover-letter"
then add to git and commit like so:
```bash
    git add .
    git commit  -m "fixed merge conflict"
```

congrats!, you just completed the exercise. if you followed the instructions step-by-step, your solution should look like what is in the "solutions" folder.

for a more detailed article on git, consider checking out [this post](https://ndiberaymond.pythonanywhere.com/posts/40/)

To learn how to make your first [free and open source](https://en.wikipedia.org/wiki/Free_and_open-source_software) contribution by adding your name to the first-contributions.md file, consider checking out this [blog post](https://ndiberaymond.pythonanywhere.com/posts/41/)