# Exercise Answers
Beginner
---
1.  
  ```
  cd ../..
  ```
2.  
  ```
  ls
  ```
3.  
  ```
  ls -l
  ```
4.  
  ```
  ls -la
  ```
5.
  ```
  mkdir clean_code_examples
  ```
6.
  ```
  touch newfile.txt
  ```
7.
  ```
   echo "I should wait to buy socks until next Fall." > socks.txt
   cat socks.txt > buy.txt
   cat buy.txt
  ```
8.
  ```
  pwd
  ```
9.
  ```
  whoami
  ```
10.
  ```
  ls ../..
  ```
11.
   ```
   touch "list of best cat pictures.html"
   ```
12.
   ```
   cd C:/Users/Default User/My Documents
   ```
13.
   ```
   ping 8.8.8.8
   ```
14.
   ```
   cd ~/documents/
   ```
15.
   	```
   	echo "My name is " $(whoami)
   	```
16.
   ```
   cat "tylers favorite songs.txt" "sarahs favorite songs.txt"
   ```
17.
   ```
   help echo > echo_options.txt
   ```
18.
   ```
   ping -n 2 127.0.0.1
   ```
19.
   ```
   cat *.md
   ```
20.
   ```
   rm yesterdays_todo_list.md
   ``` 

Intermediate
---
1.
  ```
  echo "Paritosh Balasubrahmanyam" > myname.md
  echo "Dosa, Vada, Rasmalai" >  myfavoritefoods.md
  echo "I would like to create a Simple Page Application using the latest Java
  cript that would be similar to a online clothing store" > dreamproject.md
  echo "I like classical, Instrumental and ballads. My favourite classical is
  industhani, Instrumental - Sitar and ballads of Richard Marx" > music.md
  echo "red, sky blue" > colors.md
  ```
2.
  ```
  ls -lhsS *.md
  ```
3.
  ```
  When I am in commandline-practice folder, run the following command: 
  mkdir ../backup
  tar -czf  backup1.tar.gz . | mv backup1.tar.gz ../backup/

4.
  ```
  $ echo -e 'My favorite website \n google.com \n yahoo.com \n study.moderndevelo
per.com \n' > sites.txt
```
5.
  ```
   curl study.moderndeveloper.com -L > study.html
  ```
6. 
  ```
   mv ../backup/backup1.tar  ../backup/"`date`".tar
  ```
7.
  ```
  wc dreamproject.md
  ```
8.
  ```
  grep "\.js" study.html > javascripts.html
  ```
9.
  ```
  cat *.txt | wc
  ```
10.
  ```
  tar -czf *.* > ../backup/backup2.tar
  find *.* -delete
  ```
Advanced
---
1.
  ```
  #!/usr/bin/env bash
  echo "The path of tar file is " $1
  echo "The path to extract tar file is " $2

  mkdir -p $2

  echo "Expanding path " $1 " into " $2
  echo "------------------------------"
  tar -xzvf $1 -C $2
  echo "------------------------------"
  echo "done"
  ```
2.  
  ```
  #!/usr/bin/env bash
  echo "Template will be created in folder: " $1
  echo "Title: "$2

  mkdir -p $1/css $1/images $1/js

  echo -e "<style> \r\n body{color:red;} \r\n</style>" >  $1/css/Style.css

  echo -e "<!DOCTYPE html> \r\n <html>\r\n<head>\r\n <h1><title>$2</title></h1>\r\n</head>\r\n<body>\r\n</body>\r\n</html>" >  $1/index.html

  touch $1/js/main.js

  echo "done"
  ```
3.
  ```
  #!/usr/bin/env bash

  echo "New file created: "$1
  echo "File pattern to match: "$2

  cat $2 > $1

  echo "done"
  ```
