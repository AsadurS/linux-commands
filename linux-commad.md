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
## copy file 
  - cp path/to/file_name path/from/
  - cp path/to/file_name path/from/ file _name alos remange file name 
  - scp -P 2222 path/zaman.jpg muhammad@192.168.56.1:/home/muhammad/Documents/ ( local to vps)
