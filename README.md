**CW: Command Line & Git Practice**

**Objective:**  
Students will demonstrate their ability to navigate the file system, manage files using Terminal commands, and practice using Git for version control on a Mac.

**Scenario:**  
You are a junior developer tasked with organizing a project folder for your team. Using the command line, you will create folders and files, view file contents, and manage your project using Git.

**Part 1: File System Navigation & File Management**

- Open Terminal and navigate to your Desktop:
  `cd ~/Desktop `
- Create a new project folder named cli-practice:
  `mkdir cli-practice`
- Navigate into cli-practice:
  `cd cli-practice`
- Create subfolder, notes and files:
  `mkdir notes files`
- Inside notes, create a text file commands.txt:  
  `cd notes`  
  `touch commands.txt`
- Add 5 CLI commands you learned into commands.txt:  
  `echo 'pwd' >> commands.txt`  
  (repeat for others)
- View the contents of commands.txt using `cat` and `less`
- Return to cli-practice:
  `cd ../`
- Move commands.txt to the files folder:
  `mv notes/commands.txt files/`
- Rename commands.txt to my-commands.txt:  
  `mv files/commands.txt files/my-commands.txt`
- Open my-commands.txt using the default app:  
  `open files/my-commands.txt`
- Delete notes folder:
  `rm -r notes`

**Part 2: Initialize Git and Track Changes**

- Initialize a Git repo in cli-practice:
  `git init`
- Check repo status:
  `git status`
- Add files folder to staging:
  `git add files/`
- Commit changes:
  `git commit -m 'Add my-commands.txt file with CLI practice'`
- Check commit history:
  `git log`
- Edit my-commands.txt to add another command:
  `echo 'rm' >> files/my-commands.txt`
- Stage and commit the change:  
  `git add files/my-commands.txt`  
  `git commit -m 'Added rm command to my-commands.txt'`
- View differences between commits:
  `git log -p`

**Deliverables:**  
Upload the following 3 screenshots of your Terminal onto Google Classroom:

- Final cli-practice folder structure (`ls -R`)
- Last 2 Git commits (`git log`)
- Content of my-commands.txt (`cat files/my-commands.txt`)
