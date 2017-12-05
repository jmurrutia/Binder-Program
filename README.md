# Binder Program

Team Members:  
	- Jose Urrutia (jmurrutia@csu.fullerton.edu)  
  
Part I Questions:  
	
	13.  Try opening the file using the 7-zip program.  What happens?  Are you able to extract and run the worm.bat file inside the archive?  
		- The file cannot be opened at all.  
  
	14.  After renaming the file to result.gif extension, try opening the file.  What happens?  
		- Once I renamed the file to a .gif extension, It was now able to be opened as a regular gif file.  However, the user is unaware that there is malicious code hidden within the gif file.  
  
	1.   Explain what is happening.  
		- Once I've renamed the file to a .gif extension, the file was able to be opened.  The user is unaware that that milicious code has been appended to the gif file.  This is due to the reason that operating systems use file extensions as a way of knowing what type of file it is and what program to run when opening that tpe of file.  
  
	     Do some research in order to find out what the above copy command does.  
		- The copy command has the ability to copy one or more files from one location to another, along with arguments that perform specific actions.   
  
	     In your explanation be sure to explain the role of each argument in the above command.  
		- Copy: copies one or more files from one location to another  
		- /B: indicates a binary file  
		- <.gif>: The gif file  
		- +: This command allows you to append multiple source files.  
		- <.7z>: The zip file  
		- result: name of the destination file (by default saves to origin folder)  
  
	     Also, be sure to explain how Windows handles files which leads to the above behavior.  
		- Windows looks at what type of extension the file has, and uses this information to decide which program will run the file.  
  
	2.   How can this technique be used for hiding malicious codes?  
		- This technique allows you to combine multiple files and disguise them as one.  By appending the file extension, you can confuse Windows to open that particular file using a program that can run the file extension.  A very clever way of hiding malicious code within other files.  
  
	3.   How robust is this technique in terms of avoiding detection by anti-virus tools?  You may need to do some research.  
		- It's not really robust at all, since an anti-virus program would be able to detect malware by it's own signature.  However, if this is a rather new malware program that has yet to be detected, then it is possible it can avoid detection, but not for long.  
  
Part II How to run:  
	- Enter command "python binder.py <Prog1> <Prog2> ... <ProgN>"  
		- This will create file "bound" executable  
  
	- Next, enter command "./bound"  
		- This will run the programs that were bound together  
  
Extra Credit:  
	- No extra credit attempt  
  
Special Notes:  
	- N/A  