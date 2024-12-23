**find command**

`find . -type f -name"*.php"`  
`find . -type f -iname "*.php"`  
`find . -type f -perm 0664`  
`find . -type f -size +100`  
`find . -mindepth 2 -maxdepth 2 -type f`  

**grep command**  

`grep "hello" file.txt`  
`grep -i "hello" file.txt`  
`grep -n "error" file.txt`  
`find <path> <criteria> -exec <command> {} \;`  

**Commands**  
`ls > file.txt`  
`ps aux | grep chrome`  
`pgrep` 
`kill [options] <PID(s)>`  


**Explanation:**  

`find`: The command used to search for files and directories.  
`.`:Starts searching from the current directory.  
`-type f`: Limits the search to files (not directories).  
`-name "*.php"`: Matches file names that end with .php (case-sensitive).  
`-iname` makes the search case-insensitive (e.g., it will find .php, .PHP, .Php, etc.).  
`-perm 0664`: Finds files with permissions exactly matching 0664.  
`-size`: option in the find command is used to filter files (or directories) based on their size.  
`-not` : excludes files that match the pattern *.php.  
`-mindepth 2`: Excludes the current directory from the search.  
`-maxdepth 2`: Includes only the immediate subdirectories.  
`grep`: Searches for the string hello in file.txt.    
`grep -i`: Case-Insensitive Search  
`grep -n`:Displays the line numbers of matches  
`-exec` flag in the `find` command allows you to execute a command on each file or directory that matches the search criteria. It is highly flexible and powerful for automating tasks.  
`ls`: Lists the contents of the current directory.
`>`: Redirects the output of the ls command to a file, overwriting the file if it already exists.
`file.txt`: The file where the output will be saved.  
The `ps` command is used to display information about running processes.  
The `a` option lists processes from all users.  
The `u` option provides detailed information about the processes, such as the user, CPU, and memory usage.  
The `x` option includes processes that don't have a terminal (e.g., background processes).  
This command shows all processes running on the system with detailed information.  
The pipe (|) sends the output of the command on the left (ps aux) as input to the command on the right (grep chrome).  
The pgrep command is used to search for processes based on their name or other attributes, and it returns the process IDs (PIDs) of those processes. Unlike ps combined with grep, pgrep is specifically designed for this purpose and is more efficient.  
The kill command is used to send signals to processes to control their behavior. Below are the common flags and options used with the kill command.





