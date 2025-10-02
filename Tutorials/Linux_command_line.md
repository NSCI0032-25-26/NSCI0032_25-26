# This is a brief command line intro

The following is looseley based on [the official Ubuntu Linux Manual](https://ubuntu.com/tutorials/command-line-for-beginners).

## History

See for example [AT&T Archives: The UNIX Operating System](https://www.youtube.com/watch?v=tc4ROCJYbm0)

Unix, an early multi-user operating system, ran on mainframes with simple text-only terminals that sent keystrokes to the server and displayed text output. This lightweight text interface enabled efficient interaction even over slow connections, leading to terse commands for speed. Users managed files and executed tasks through a “shell,” which allowed command chaining, wildcards, and automation via shell scripts. Modern Linux systems inherit this Unix design, still using text based shells, however now typically in software terminals within graphical environments!

## Advantages

- Speedy and Resource Efficient
    Text-based tools run faster and use fewer resources than heavy GUIs
- Automation & Reproducibility / Repeatability 
    Shell scripts allow you to automate repetitive tasks and create reproducible pipelines
- Integration with Modern Tools
    Seamlessly and readily integrates with state of the art data science tools (Python,  Hadoop)  making it the backbone of cloud and HPC environments
- Scalability & Remote Work
    When working on clusters or cloud platforms, you often don’t have a GUI, or it is slow, command-line skills are essential!
- Industry Standard
    Every major data science platform (AWS, GCP, Azure) expects familiarity with the shell for deployment and automation
- It is like a meta or super programming language that connect different programmes into power pipelines...

## Task 1: Open a Terminal

Follow the instructions in class !

![4df91aee64a67e357a4de3ae72667372.png](:/0808c9a5163148b2ac3f5660e8fc3346)

&nbsp;

## Task 2

Let’s run our first command.

Click the mouse into the window to make sure that’s where your keystrokes will go, then type the following command, all in lower case, before pressing the Enter or Return key to run it.

`pwd`

You should see a directory path printed out (probably something like /home/YOUR_USERNAME), then another copy of that odd bit of text.

&nbsp;

![06dc0b325899f8334221ebac239c5351.png](:/c77b19aa9d00476b942e2bd37a3aa684)

## The Prompt

It is this odd piece of text that appear after every command.. it is a way for the computer to tell you (prompt you) that it is ready for the next commend. 

Note: you can customise the prompt, for example to display time, or current folder, or programme, etc, tip: Ask your favorite bot to customise it for you! 

## Where are we?

ok, so `pwd` is  an abbreviation of ‘**p**rint **w**orking **d**irectory’.

You can change the working directory using the `cd` command, an abbreviation for ‘**c**hange **d**irectory’. Try typing the following:


```
cd /
pwd


```

This leads you to the top folder (directory) of the file system, it is called the ROOT

this command
```
cd home
pwd
```

will send you back to the home folder!

To go up to the parent directory, in this case back to “/”, use the special syntax of two dots ``..`` when changing directory (note the space between `cd` and `..`

### Task
Lets is wonder arround together in the file system...

## Creating folders and files


mkdir /tmp/tutorial
cd /tmp/tutorial

mkdir dir1 dir2 dir3


what happens when you try to pass the wrong number of parameters to a command:

mkdir
cd /etc ~/Desktop

# The most common command ...

ls

![8dd2f7a93d1d5cf870b49e769e3fd4f3.png](:/126bdc9457ce47fbb24ea3ae8ee7b992)



### what does this do?
mkdir -p dir4/dir5/dir6
ls

## Creating files using redirection

we can redirect the output of one command to a file, or even to another comman or application

ls
ls > ls.output

cat ls.output


## we will continue interactively in the class!
