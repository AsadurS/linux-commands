# linux-commands
  ## listing
    -ls (list all file and folder)
    -ls -l (long list mean list with details)
    -ls -h (list with human readable )
    -ls -a (list with hidden file folder)
    - ls -d <file folder name>(show specefic file folder details)
    - ls -r (reverse order)
    - ls -t (Sort by modification time, displays files and directories in order of their last modification time, with the most recently modified first)
    - ls -S (Sort by file size, displays files and directories in order of their size, with the largest first)
    - ls --help(get All ls Command)
    - ls -lu accstime
 ## cd -Change directory
    - cd /path/want/to/go
    - cd .. (Moves up to the parent directory)
    - cd ~/Documents (Moves to the "Documents" from anyware)
    - cd  (Shortcut to home directory)
    -cd - (Switches to the previous directory)
## create directory
    - mkdir <dir_name>
    - mkdir <dir1 dir2 dir3>(multiple directory)
    -  mkdir -v <dir> show message
    - mkdir -p path/to/new/directory chaning direcotry
    -chmod permissions directory_name
    - mkdir -m a=rwx <dir>(with permission)
## remove direcory
  -rmdir <dir_name>
  -sudo rm -rf <directory/> with sub folder or folder not emty
## create  file 
   - touch <file_name> single file create
   - touch <file_1 file_2 file_2> multile file create
   - rm <file_name file_1> for remove multiple and singel
## show file 
  - cat file_name
  - cat file1.txt file2.txt(concat multiple file)
  - cat -n test.txt show with line number
## copy file file folder
  - cp path/to/file_name path/from/
  - cp path/to/file_name path/from/ file _name alos remange file name 
  - scp -P 2222 path/zaman.jpg muhammad@192.168.56.1:/home/muhammad/Documents/ ( local to vps)
  - scp -r -P 2222 C:/Users/SAMSUNG/Downloads/local muhammad@192.168.56.1:/home/muhammad/Documents/ (local to vps folder)
  - scp -r -P 2222 muhammad@192.168.56.1:/home/muhammad/Documents/ C:/Users/SAMSUNG/Downloads/local (vps to local )
## move file folder
  -mv source_file /path/to/des(move)
  - mv old_name new_name (rename file)
  - mv new_folder/ ~/Downloads/ (move folder)
## Zip a unzip
  - zip <zip_file_name.zip> file_folder_wich_want_to_zip
  - zip all file_one  folder (zip file and folder together)
  - zip -r archive.zip directory/ -x "*.ts" "*.tmp"(Create a zip archive, excluding specific files)
  - unzip archive.zip -d /path/to/destination/ (unzip to destination)
## create user 
   - su (switch user) sudo su  mean change user to root
   - sudo adduser username(create user)
   - adduser -g <group_name> -s /bin/bash(for bash sell) -c "command or desciprtion " -m (create home directory or not) -d /home/dir_name <username>
   - sudo userdel username(delete user)
   - sudo userdel -r username(delete user with home directory)
   - sudo userdel -f username(delete user if user logind)
   - sudo pkill -KILL -u <username> (if user is login u can logout using this command)
   - cat /etc/passwd (show users)
## Group 
  - sudo groupadd <group_name>
  - sudo groupdel <user name>
  - cat /etc/group (show groups)
## usermod
  - usermod -aG <group_name> <user_name> (remove previous group add new group)
  - usermod -g <group_name> <user_name> (remove previous group add new group)
  - usermod -G <group_name> <user_name> (add user group with previous group)
  - sudo usermod -m -d /new/home/directory username (Change the user's home directory with all data)
  -  sudo usermod -l newusername oldusername (Change the user's login name)
  -  sudo usermod -G group1,group2 username (Add the user to additional groups)
  -  sudo usermod -L username (Lock a user account)
  -  sudo usermod -U username (Unlock a previously locked user account)
