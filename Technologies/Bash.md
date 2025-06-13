---
type: documentation
technology: programming_language
devops: ✅
---
#technology 
# Description
**Bash (Bourne Again Shell)** is a command-line interpreter and scripting language that serves as the default shell for most Linux distributions and macOS systems. Originally developed by Brian Fox for the GNU Project as a free replacement for the Bourne shell, bash has become one of the most widely used shells in Unix-like operating systems.

As a command-line interface, bash allows users to interact with their operating system by typing commands directly into a terminal. You can navigate directories, manipulate files, run programs, and perform system administration tasks through simple text commands. For example, `ls` lists directory contents, `cd` changes directories, and `grep` searches through files.

Beyond basic command execution, bash is a powerful scripting language that enables automation through shell scripts. These scripts can combine multiple commands, use variables, implement conditional logic with if-statements, create loops, and define functions. This makes bash invaluable for automating repetitive tasks, system administration, deployment processes, and data processing workflows.

# Notes and Good Practices

## Processes and background
In order to put a process in the background there are multiples way :
The most command is the `&` at the end of the command.

But we can also use the `bg` command. For that we can use `Ctrl+z` to stop the current process. Then hitting `bg` will but it in the background and `fg` to put it back to the foreground.

A good command to know in this kind of situation is `nohup`. When used before a command it will unsure that the command is still running even if the user who launch the command is disconnected. It was used [[2025-06-13]] with GitHub Runner processes. for that its good to use it with the `&` like that : `nohup <command> <input> &`.

Also instead of using `ps aux` it can be good to use `ps -ef` or `top -c` or `pstree` to check the process with still seeing there parent process and then having a good view of the tree cand what to kill if needed.

