# Setup Flake8 in PyCharm



1. Go to menu File > Settings. In Tools > External Tools, add a new tool.

   <img src="https://raw.githubusercontent.com/qinjie/picgo-images/main/image-20211113003041566.png" alt="image-20211113003041566" style="zoom:67%;" />

    

2. Edit the Tool settings as following:

   * Name: `Flake8`

   * Program: `$PyInterpreterDirectory$/python`

   * Arguments: `-m flake8 --max-complexity 10 --ignore E501 $FilePath$`

   * Working directory: `$ProjectFileDir$`

   * Output Filters:

     ```
     $FILE_PATH$\:$LINE$\:$COLUMN$\:.*
     $FILE_PATH$\:$LINE$\:.*
     ```

   <img src="https://raw.githubusercontent.com/qinjie/picgo-images/main/image-20211113003144619.png" alt="image-20211113003144619" style="zoom:80%;" />

   

   3. Go to menu Tools > External Tools > Flake8 to run the check on current file.

   