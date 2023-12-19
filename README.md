internsctl is a custom Linux command designed to simplify various server operations. This bash script provides functionality for retrieving server information, managing users, and obtaining file details. The current version is v0.1.0.
Installation
To install internsctl, you can use the following steps:
        $ git clone https://github.com/your-username/internsctl.git
        $ cd internsctl
        $ make install
Usage
Manual Page
To view the full documentation of the command, use the man command as follows:
        $man internsctl
This will display detailed information about the command, including usage guidelines and available options.
Help
To get help and see examples of how to use internsctl, use the --help option:
        $ internsctl --help
This will provide you with a summary of the command's usage, options, and examples.
Version
To check the version of internsctl, use the following command:
        $ internsctl --version
This will display the current version of the tool.

Section B
Part 1 | Level Easy
Get CPU Information
To get CPU information of your server, use the following command:
      $ internsctl cpu getinfo
Expected Output: Similar to the output from the lscpu command.

Get Memory Information To get memory information of your server, use the following command:
      $ internsctl memory getinfo
Part 2 | Level Intermediate
Create a New User
To create a new user on your server, use the following command:
      $ internsctl user create <username>
Note: The above command will create a user who can log in to the Linux system and access their home directory.

List All Users
To list all regular users on your server, use the following command:
        $ internsctl user list
List Users with Sudo Permissions
To list all users with sudo permissions on your server, use the following command:
        $ internsctl user list --sudo-only
Part 3 | Advanced Level
Get File Information
To get information about a file, use the following command:
        $ internsctl file getinfo <file-name>
File Information with Options
To obtain specific information about the file, use options as follows:

To print the size of the specified file:
          $ internsctl file getinfo --size hello.txt
To print file permissions:
          $ internsctl file getinfo --permissions hello.txt-rw-r--r--
To print file owner:
          $ internsctl file getinfo --owner hello.txt xenonstack
To print the last modified time:
          $ internsctl file getinfo --last-modified hello.txt 2020-10-07 20:34:44.616123431 +0530









