# UOCIS322 - Project 0

Trivial project to exercise version control, turn-in, and other mechanisms 
for CIS 322, introduction to software engineering at the University of Oregon.

:warning: Be careful about the changes you make.
I highly recommend waiting until session 2 (04/08/2021).
If you insist on getting started earlier, please let me know
so I can explain everything in advance.
The best way to reach me is through Slack or email.

## Before you begin

If you don't know how to SSH:

```
ssh your_cs_username@hostname
```

If you're using Windows, please refer to this [link](https://www.howtogeek.com/336775/how-to-enable-and-use-windows-10s-built-in-ssh-commands/) for instructions on enabling SSH in Windows.

An alternative for all platforms: [Termius](https://termius.com/).

In order to access your GitHub repos and commit changes from the server,
make sure you set up an SSH key first. 
[Tutorial](https://docs.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent).

When you're done, use the following command to add the key (do this every time you SSH into the server):
```
ssh-add path/to/.ssh/ssh_filename
```
If you're doing this locally (on your own device and not testium), and you're not using Linux, please pay attention to the Tutorial link above.

## Instructions

- Start by forking this repository on
[GitHub](https://github.com/alihassanijr/UOCIS322-P0),
then cloning onto the server. Read this file (README.md). 
  
- Before you edit a file, read the comments (inside that file) carefully.

- Copy the credentials-skel.ini file, rename it to credentials.ini and fill in
  appropriately.

- Modify the program "hello.py" so that it prints "Hello
  world". (Nothing more and nothing less.)  Note that you do NOT do
  this by DIRECTLY adding the message to the hello.py source file.
  Rather, the message is a configuration constant from the credentials.ini file;
  fix it there.


Author: Derek Pinto, dpinto@uoregon.edu
Program outputs "hello world"

- Test your program locally; revise and re-test as needed. (How long
  can it take, really?)

- Commit your changes. You will need to use "git add" on your files
   hello.py and README.md, but *not* on credentials.ini, because that
   file does not belong on bitbucket.  (In later projects it will contain
   confidential information, like access keys and passwords for web
   services.)  Your changes must be "pushed" to your public repository
   on bitbucket so that the auto-checker can "clone" them back to the
   grading machine.

- Test your code with the Makefile. Use the command ``make run`` to execute.
Revise and push changes as needed.

- Turn in with Canvas. The file you turn in is credentials.ini. We
   use the repository link in your credentials.ini to access the rest,
   just like the auto-checker.
