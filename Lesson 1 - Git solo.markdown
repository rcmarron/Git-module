#Git - using git alone
__Goal:__ To teach the basics of git and why git is useful for an individual to use. This does not touch any of the server pieces.

__Overview:__ Throughout the lesson, we use examples from writing a paper to explain a git repository. Concepts explained are:
* Why you want a versions control system
* Git basics
	* Directory
	* Repository
	* Git init
	* Git status
	* Git add
	* Commits and commit messages
	* Git revert
* Git exercise

##Why you want a versions control system
Using an example, explain a scenario where someone may change something and then want to get back to the original. This example should be something the students can relate to. For this example, below, I am using the scenario of writing a paper.

__Teacher:__ How many of you have ever written an essay by hand?

__Students:__ [All raise their hands]

__Teacher:__ Stand up if you have ever been writing an essay, and you decide a something is not good. So you erase it?

__Students:__ [A bunch of the students stand up]

__Teacher:__ Stay standing, if you have ever wanted to get the thing you erased back. Maybe you realized that one of the sentences was great, or maybe you realized you never should have erased any of it.

__Students:__ [Some sit down]

__Teacher:__ Anybody want to share their story?

__Student:__ [A student tells a story about wanting to get their deleted content back]

__Teacher:__ How many of you have ever done the same thing on a computer? You typed something, deleted it, and then wanted it back.

__Students:__ [A bunch raise their hands]

__Teacher:__ Can you guys think of any ways that we could solve this problem on a computer? [If needed, give a hint of "maybe something with the way you save files"]

__Students:__ [Come to the idea of saving old files as different names]

__Teacher:__ This would work, and it is what we call versioning. Do you guys all know what versions are?

__Students:__ [Someone explains what versions are]

__Teacher:__ [Draw an example of a file versioning - show adding many files and how it gets messy]

__Teacher:__ Do you guys think this would be a good way of doing things?

__Students:__ No

__Teacher:__ Do you guys remember the different files that you used to make a website?

__Students:__ Yes, Index.html, style.css, P5.js etc.

__Teacher:__ How confusing would it be if you kept renaming your files and adding more to the folder. You would have StyleV1.css - StyleV20.css. Not only that, but you would need to change each reference to that file as you rename the latest version. A big mess huh?

__Teacher:__ Fortunately, some smart people invented "a version control system" to solve this. 

## Git basics

__Teacher:__ A version control system is a computer program. Its job is to create versions of your files without renaming them. There are many different types of version control systems. The one we are going to learn is "Git".

### Directory

__Teacher:__ There are a couple basic concepts behind Git that we need to understand. The first is a directory How many of you know what a directory is?

__Students:__ [Explain what a directory is - if they struggle, explain the  mkdir terminal command.]

__Teacher:__ Git is able to to create something called a repository within a directory. Do you guys know what a repository is?

__Students:__ [Someone may talk about a water repository...]

__Teacher:__ A repository is a computer term for an area that tracks objects. So, you can create a git repository within a directory. And what do you think this Git repository does?

__Students:__ [It tracks things within the repository]

__Teacher:__ Exactly, the git repository will track any object that is inside it. For example, if you have a file inside the directory, and you add it to the repository, the repository will track it. What about the file do you think the repository would track?

__Students:__ [It would track changes to the file]

__Teacher:__ Correct, for example, if you add a file to the repository, it will track that change. If you change anything within that file, it will track that change too.

__Teacher:__ Ok, so now we have a repository and are tracking some files within the repository. The question comes up about how frequent these changes should be tracked. You need to balance how cluttered the history would be while still allowing you to get back to important parts of your document. To do this, git has a concept called a "commit". All it is is a version or a picture of the repository at a specific time.

__Teacher:__ So now we know about:
* Directories
* Repositories
* Commits
The next part is to learn how to use them in the command line.

To use any of the git commands, the command needs to start with the word "git." For example, to create a git repository, the command is "git init". Does anyone know what "init" stands for?

__Students:__ Nope

__Teacher:__ It means initialize. Does anyone know what initialize means?

__Students:__ It means to start or create

__Teacher:__ Exactly, so "git init" means: git create - so it tells the computer to create a git repository.

So lets do that. We navigate to the directory that we want to create a Git repo in, and we create it.

Now, we want to add some files to the git repository. But before we can do that, we need to create those files. Who knows how to create a file?

__Students:__ I do! "gedit <filename>"

__Teacher:__ Perfect, now we have a file created, but it is in the directory and not in the repository. How do you think we could add it to the repository? 

__Students:__ No clue

__Teacher:__ Well what do we know all git commands start with?

__Students:__ "Git"

__Teacher:__ Right, and what do we want to do?

__Students:__ Add a file to the git repo

__Teacher:__ Right, so do you think "Git add" would work? Lets give it a shot. We would write "git add <filename>

Cool, so now we have a file living in the repository, but we haven't made any commits yet. To do that, we would need to use the command "git commit -m "<message>""

The message is used to describe what has changed in this new version or commit.

Notice the SHA that is created when we run the command. This is the unique identifier for this commit. It behaves like the commit's name.

So now that we have this file and it is commited to the repository, lets make some more changes and commit it.

[get some changes and commit]

Now, say we no longer want those changes. To fix this, we could use the command "git revert 0766c053..HEAD". Lets walk through exactly what this says. 

Now, to create a new version here, we would need to use "git commit"

As an exercise, lets all go to the computers and:

* Create a directory
* Create a git repository
* Add a file to the git repository
* Commit those changes
* Make some more changes
* Commit again
* Revert back to the first change
* Commit again


















