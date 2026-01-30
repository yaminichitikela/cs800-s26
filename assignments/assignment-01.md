# Assignment 1, Course Setup and RCR
## CS 800 Research Methods, Spring 2026

Due: 2026-02-02

Points available: 10

This assignment will cover the necessary steps to get set up for the semester and will have you complete training required for all ODU graduate students.  Read over the entire assignment before starting and make sure to read the information in the linked webpages.
The HTML skills are easy and will be used in later assignments when you create a home page for yourself.  Otherwise, the purpose of this assignment is to familiarize you with the basic mechancis of Git/GitHub, Markdown, and Youtube.

*For this assignment only -- you may ask others in the class for help with these setup tasks.  Please use our Blackboard Discussion Board Q&A Forum for these questions so that others may benefit from the answers.*


### Basics of HTML, Git, GitHub

* I've also submitted a (partial) version of what your submission should look like; consult [Nelson/1](Nelson/1) if you are unsure what things should be named, what to upload, etc.  

### Using npm to download "workshops" about HTML, JavaScript, and Node

On your computer, use npm to globally ("-g") install these packages:

```
npm install -g learnyouhtml 
```

You can omit "-g" if you don't want to install them globally, but it's probably better to make them global.

### Setting Up GitHub

Set up an account on GitHub.  Go to [https://github.com/phonedude/cs800-s26](https://github.com/phonedude/cs800-s26) and click the "Fork" button (top right).  This will create a copy of my repository in your GitHub account.  But the files nave not been moved to your local machine.  To do that, open a terminal window (replace YOURGITHUBACCTNAME (mine is "phonedude") with the name of your GitHub account):

```
git clone https://github.com/YOURGITHUBACCTNAME/cs800-s26.git
cd cs800-s26
```

This has now moved a copy of your fork of my repo from github.com to your local machine, where you will do your programming, development, testing, etc.  

### Preparing Assignment 1 for Submission

This assumes you're already in the copy of your repo on your local machine; YOURLASTNAME is your last name (mine is "Nelson")):

```
cd assignments
mkdir YOURLASTNAME
cd YOURLASTNAME
mkdir 1
cd 1
mkdir html
cd html 
learnyouhtml
# do all the HTML excercises in the "html" directory; saving all related files in "html"
cd ..
```

The command "learnyouhtml" will have you do a series of simple exercises to prove mastery of the particular task.  Each task will have you create a file, then you'll "verify" the file, and the workshop will check it.  If you're successful, it will mark that task as "[COMPLETED]".  Else, it will provide hints as to why it was unsuccessful and you re-verify after editing.  For example, to verify the HTML "lists" tasks, do:

```
cd html
learnyouhtml
vi my-list-demo.html # create the file with the desired <ul>, <ol>, <li>, etc. elements
learnyouhtml verify my-list-demo.html
learnyouhtml # to choose the next task
```

The HTML workshops is pretty easy, so you should have no problems.  Ask the email list if you get stuck.  

### Submission

* Create a README.md that contains:
  * A description of the assignment, directories, files, etc.
  * A screen shot showing completion of learnyouhtml
  * A link to a Youtube video showing you list the files in the directory and showing the end screen for the workshop.

Again, look at [Nelson/1](Nelson/1) for a template.

To upload to GitHub, do:

```
git add 1 # this will recursively add all the files in the directory
git commit -m "A1 submission" # or whatever mesg is appropriate
git push origin main # this moves the code from your local machine to github.com
```

Then inspect in your fork on GitHub (e.g., https://github.com/YOURGITHUBACCTNAME/cs800-s26).  If all looks good, issue a pull request (PR) to my repo (see [week 1 slides](https://docs.google.com/presentation/d/1w_90xM9p4Kz7Q7b-kUWCr9Gcl93u1rIQdw1YQANsoF8/edit) for details).

The idea is to collect all of the code, images, documentation, etc. necessary for someone to understand Assginment 1 into a single directory.  If it is code, data, etc. that you created, move it somewhere into ```assignments/YOURLASTNAME/1```.  We will follow this pattern for all assignments.

After the assignment is complete, you can optionally uninstall the package with:

```
npm rm -g learnyouhtml 
```

### Youtube video

* Record your screen of you 1) viewing the files, and 2) executing each of the three commands to show completion.  I am issuing grades based on what your video shows; if you don't show/demonstrate something in your video, I'm not grading it.  
* Upload that video to Youtube (see [week 1 slides](https://docs.google.com/presentation/d/1w_90xM9p4Kz7Q7b-kUWCr9Gcl93u1rIQdw1YQANsoF8/edit))

