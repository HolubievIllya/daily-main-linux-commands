## Commands
## ls command
List files and folders in the current directory.
<p>Parameters:</p>
<ul>
  <li><b>–l</b> to list the content as a detailed list</li>
  <li><b>-a</b> display all files (hidden + non-hidden)</li>
  <li><b>-r</b> reverses the sorting order for the displayed files and directories</li>
  <li><b>-s</b> sorts the output by file size</li>
  <li><b>-t</b> sorts the output by file modification time</li>
</ul>
<p>Example of input: <b>ls -la</b></p>


## pwd command
Shows current directory
<ul>
  <li><b>-L</b> prints the symbolic path</li>
  <li><b>-P</b> prints the actual path</li>
</ul>
<p>Example of input: <b>pwd</b></p>


## cd command
Change directory from the current directory to another one.
<ul>
  <li><b>~</b> back to main directory</li>
  <li><b>..</b> move to the parent directory</li>
</ul>
<p>Example of input: <b>cd /home</b></p>

## touch command
The touch command is used to create an empty file.
<p>Parameters:</p>
<ul>
  <li><b>–t</b> creates file followed by the time with the following format YYYYMMDDHHMM</li>
  <li><b>-a</b> changes file access and modification time</li>
  <li><b>-c</b> does't create n empty file</li>
</ul>
<p>Example of input: <b>touch -t 202012011200 test1</b></p>

## rm command
You can easily delete single files
<ul>
  <li><b>–i</b> will ask before deleting each file</li>
  <li><b>–r</b> will recursively delete a directory and all its contents (normally rm will not delete directories, while rmdir will only delete empty directories)</li>
</ul>
<p>Example of input: <b>rm name</b></p>

 
## cp command
Copy the source to target.
<p>Parameters:</p>
<ul>
  <li><b>–i</b> interactive mode means waiting for the confirmation if there are files on the target, it will be overwritten</li>
  <li><b>-r</b> recursive copy means include subdirectories if they found</li>
  <li><b>-u</b> оverwrites the destination file only if the source file is newer than the destination file</li>  
</ul>
<p>Example of input: <b>cp –ir sourcedir targetdir</b></p>


## mv command
Move the source to target and remove the source.
<p>Parameters: </p>
<ul>
  <li><b>–i</b> interactive mode means to wait for the confirmation if there are files on the target, it will be overwritten</li>
  <li><b>–f</b> does not prompt you before overwriting an existing file</li>
</ul>
<p>Example of input: <b>mv –i sourceFile targetFile</b></p>


## rm command
Delete file or directory, and you must use –r in case you want to delete a directory.
<p>Parameters:</p>
<ul>
  <li><b>–r</b> recursive delete means delete all subdirectories if found</li>
  <li><b>-i</b> interactive means wait till confirmation</li>
</ul>
<p>Example of input: <b>rm –r anotherDir/</b></p>


## mkdir command
Create a new directory.
<ul>
  <li><b>-v</b> prints a message for each created directory</li>
  <li><b>-m</b> set file mode</li>
</ul>
<p>Example of input: <b>mkdir NewDir</b></p>


## rmdir command
Delete a directory.
<ul>
  <li><b>-p</b> removes the directory, including all its ancestors</li>
  <li><b>-v</b> displays verbose information for every directory</li>
</ul>
<p>Example of input: <b>rmdir NewDir/</b></p>


## chown command
Change the owner of a file or directory.
<p>Parameters:</p>
<ul>
  <li><b>–R</b> capital R here means to change ownership of all subdirectories if found, and you must use this parameter if you use the command against a directory</li>
  <li><b>-f</b> suppresses all error messages except usage messages</li>
</ul>
<p>Example of input: <b>chown –R root:root myDir</b></p>


## chmod command
Change the permission of a file or directory.
<p>Parameters:</p>
<ul>
  <li>The mode which consists of 3 parts, owner, group, and others means what will be the permissions for these modes, and you must specify them</li>
  <lihe mode which consists of 3 parts, owner, group, and others means what will be the permissions for these modes, and you must specify them.

The permission is one of the followings:

Read =4

Write = 2

Execute =1

Every permission represented by a number as shown, and you can combine permissions.</li>
</ul>
<p>Example of input: <b>chmod 755 myfile</b></p>
That means set permission for the file named myfile as follows:
owner: set it to 7, which means 4+2+1 means read+write+execute.
group: set it to 5, which means 4+1 means read+execute.
other: set it to 5, which means 4+1 means read+execute.
Note: execute for a folder, means opening it.


## locate command
To find a file in your system, the locate command will search the system for the pattern you provide..
<p>Example of input: <b>locate myfile</b></p>


## date command
Simply prints today’s date. Just type date on the shell.
<ul>
  <li><b>-I</b> displays the date and time in ISO 8601 format</li>
</ul>
<p>Example of input: <b>date</b></p>


## find command
Finds all files with flags you provided.
<ul>
  <li><b>-type</b> filter by file type</li>
  <li><b>-name</b> filter by file name</li>  
</ul>
<p>Example of input: <b>find . -type f -name "*.txt"</b></p>


## echo command
Used to display line of text/string that are passed as an argument.
<ul>
  <li><b>-n</b> used to omit echoing trailing newline</li>
  <li><b>-e</b> enables the interpretation of backslash escapes</li>  
</ul>
<p>Example of input: <b>echo "Hello, world!"</b></p>


## df command
Displays the disk space used in the file system.
<ul>
  <li><b>–h</b> displays space in gb and mb</li>
  <li><b>-c</b> displays the output in colon separated format</li>  
</ul>
<p>Example of input: <b>df"</b></p>


## tar command
Combines several files into an archive and compression if you want.
<ul>
  <li><b>–c</b> create a new archive</li>
  <li><b>-z</b> compress the archive using gzip package</li>
  <li><b>-j</b> compress the archive using the bzip2 package</li>
  <li><b>-v</b> verbose mode means showing the processed files</li>
  <li><b>-f</b> write the output to a file and not to screen</li>
  <li><b>-x</b> unpack files from an archive</li>
</ul>
<p>Example of input: <b>tar –czvf myfiles.tar.gz myfiles</b></p>
This command will pack and compress all files in folder myfiles to a compressed archive named myfiles.tar.gz.
<p>Example of input: <b>tar-xzvf myfiels.tar.gz</b></p>
This command will decompress the archive.


## cat command
Displays file content to screen without limits.
<ul>
  <li><b>-n</b> displays line numbers in front of each line in a file</li>
  <li><b>-b</b> removes the empty lines</li>  
  <li><b>-е</b> displays a '$' sign at the end of every line</li>   
</ul>
<p>Example of input: <b>cat myfile.txt</b></p>

 
## tail command
Output the end of a file
<ul>
  <li><b>-n num</b> prints the last ‘num’ lines instead of last 10 lines</li>
</ul>
<p>Example of input: <b>tail test.txt</b></p>


## more command
Command is used to view the text files in the command prompt.
<ul>
  <li><b>–p</b> clears the screen and then displays the text</li>
  <li><b>-n</b> option displays the line numbers at the beginning of each line</li>
  <li><b>–s</b> squeezes multiple blank lines into one single blank line</li>
</ul>
<p>Example of input: <b>more -p sample.txt</b></p>


## less command
Displays file content with a scroll screen so you can navigate between pages using PgUp, PgDn, Home, and End.
<p>Example of input: <b>less myfile</b></p>


## head command
<ul>
  <li><b>–n</b> prints a specific number of lines from the beginning of a file</li>
  <li><b>–c</b> prints a specific number of bytes from the beginning of a file</li>
  <li><b>–v</b> data from the specified file is always preceded by its file name</li>
</ul>
<p>Example of input: <b>head -n 5 sample.txt</b></p>


## grep command
Searches for a string in the specified files and displays which line contains the matched string.
<ul>
  <li><b>–R</b> recursive search inside subdirectories if found</li>
  <li><b>-i</b> insensitive search and ignore case</li>
  <li><b>-l</b> displays file name, not the text lines</li>
</ul>
<p>Example of input: <b>grep "print" main.py</b></p>


## diff command
Allows you to compare two files line by line.
<ul>
  <li><b>–c</b> allows you to view additional information related to the specified files and the changes needed to make them identical</li>
  <li><b>-u</b> it avoids displaying redundant information</li>
</ul>
<p>Example of input: <b>diff text1.txt test2.txt</b></p>


## comm command
Compare two sorted files line by line and write to standard output.
<p>Example of input: <b>comm text1.txt test2.txt</b></p>

## passwd command
Used to change your user password.
<p>Example of input: <b>passwd</b></p>


## du command
Calculates the disk usage of a file or a directory.
<ul>
  <li><b>–h</b> display human-readable form</li>
  <li><b>-s</b> summarize the output total size</li>
  <li><b>-a</b> lists the sizes of all files and directories in the given file path</li>  
  <li><b>-c</b> adds a line to the bottom of the output that gives you a grand total of all of the disk usage for the file path given</li>    
</ul>
<p>Example of input: <b>du –hs /home</b></p>


## reboot command
Reboot the system immediately.
<p>Example of input: <b>reboot</b></p>


## screen command
Provides the ability to launch and use multiple shell sessions from a single ssh session.
<ul>
  <li><b>–A</b> it force all capabilities into each window’s termcap</li>
  <li><b>-S</b> creates a named session</li>  
</ul>
<p>Example of input: <b>screen -a</b></p>


## halt command
Shuts down the system, but make sure to close all of your files to avoid data loss.
<p>Example of input: <b>halt</b></p>


## ps command
The ps command lists the currently running process.
<p>Example of input: <b>ps aux</b></p>


## pkill command
Kill a process.
<p>Example of input: <b>pkill processName</b></p>


## nano command
You can edit file, if it doesn't exist command will create new one
<p>Example of input: <b>nano</b></p>

## Get the version of GTK
<p>Example of input: <b>dpkg -s libgtk-3-0|grep '^Version'</b></p>


## sudo command
Runs command as superuser
<p>Example of input: <b>sudo touch</b></p>


## top command
Provides with information about all running processes
<p>Example of input: <b>top</b></p>


## free command
Shows memory usage
<p>Example of input: <b>free -h</b></p>


## tree command
Shows the hierarchy of files and folders in directory
<ul>
  <li><b>-f</b> prints the full path prefix for each file</li>
  <li><b>-i</b> ignores case when sorting filenames</li>  
</ul>
<p>Example of input: <b>tree</b></p>


## ping command
Shows the ping of the website
<ul>
  <li><b>-c amount</b> display ping amount time</li>
</ul>
<p>Example of input: <b>ping www.google.com</b></p>

## netstat command
Show all open connections on your pс
<ul>
  <li><b>-D</b>  allows you to see packets coming into and going out of each layer in the communications subsystem along with packets dropped at each layer</li>
</ul>
<p>Example of input: <b>netstat</b></p>

## ifconfig command
Shows ip and etc of your pc
<p>Example of input: <b>ifconfig</b></p>

## w command
Shows all users on your machine
<p>Example of input: <b>w</b></p>

## wc command
Finds out the number of newline count, word count, byte and character count in the files specified by the File arguments
<ul>
  <li><b>-l</b> prints the number of lines in a file</li>
  <li><b>-w</b> prints the number of words in a file</li>
  <li><b>-c</b> displays the count of bytes in a file</li>
  <li><b>-m</b> prints the count of characters from a file</li>
  <li><b>-L</b> prints only the length of the longest line in a file</li>
</ul>
<p>Example of input: <b>wc -L</b></p>


## shuf command
Writes a random permutation of the input lines to standard output.
<ul>
  <li><b>-n</b> prints the number of lines in a file</li>
</ul>
<p>Example of input: <b>shuf -n 25 hello.txt</b></p>

## cmp command
Allows you to check if two files are identical.
<ul>
  <li><b>-b</b> prints differing bytes</li>
</ul>
<p>Example of input: <b>cmp hello.txt test.txt</b></p>
