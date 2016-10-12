#Instructions for Running a Text Editor from GIt Bash on Windows 10

These instructions assume that you already have already downloaded and installed Git Bash and Sublime for Windows 10. I have not attempted this with other text editors, but I hazard to guess the instructions are similar. These instructions are culled from Stack Overflow and Here.

In order to execute your text editor from Git Bash (not the default bash on Windows), open up Notepad and create the following file named Subl:
#!/bin/sh
"C:\Program Files\Sublime Text 3\sublime_text.exe" $1 &
In the above block of code, the line between “…” is the path where your text editor executable is installed. Save Subl wherever you want. I recommend to your desktop, so it is easy to find. Notice that Subl is likely saved as a text (Subl.txt) file. We want to get rid of the extension. However, the Windows gui doesn’t allow us to access the file extensions, so we have to do the following steps.

Next, run the Window’s command terminal (cmd) as an administrator. Navigate to where you saved Subl.txt (i.e. C:\Users\Andrew\Desktop). We want to get rid of that .txt extension. Use the copy command as follows:
C:\Users\…\Desktop>copy Subl.txt Subl
Now we have Subl with no extension. We now want to move it into our Git Bash bin directory, so that when we type Subl new_text_file.txt in Git Bash, it opens up new_text_file.txt using Sublime or your particular text editor. 

First, find the path of where your Git Bash bin directory is. The path is likely C:\Program Files\Git\usr\bin or “C:\Program Files (x86)\Git\bin” depending on if you did the 64 or 32-bit installation. Still in the Windows command terminal (running as an administrator), type the following: 
C:\Users\...\Desktop>move Subl “C:\Program Files\Git\usr\bin”
If you want, you can combine the above step with the previous step. This has now moved the script Subl to the specified bin directory. Now, in Git Bash you should be able to simply type Subl new_text_file.txt and it will create (if it doesn’t yet exist) or open up new_text_file.txt using Sublime. 

I have not tested this for any other text editor (i.e. nano/vim/atom/etc), but I imagine a similar script in similar directories should have similar results. 
