    1  #!/bin/bash
    2  if [ -z $1 ]; then    echo "well, someone didn't want to run the script with a file...";   exit; fi
    3  #!/bin/bash
    4  if [ -z $1 ]; then    echo "well, someone didn't want to run the script with a file...";   exit; fi
    5  file=$1
    6  bug=7c85d987a917c2a555d1391426978f05
    7  mesg="Level 7: \n Linus has been here...\nI love messing with these amateur programmers!!\nIf you want some real fun, then you should try resolving a conflict between this branch (tree) and code4life.\nI introduced a little bug that you should fix in the conflict. >:)\nAfter you merge these 2 files you should run the shell script again!!\n\nGood Luck!!!\n\n Hint: https://help.github.com/articles/resolving-a-merge-conflict-from-the-command-line/ "
    8  merges=$(git log --format=%h --merges | head -1)
    9  csum="md5sum"
   10  if [ $(echo "$OSTYPE" | grep darwin) ];then     csum="md5"; fi
   11  if [ "$file" = "nextclue_input.cpp" ];then    if [ ${merges} ]; then      while read p; do        for w in $p;do          if [ `echo $w | $csum | awk '{print $1}'` = $bug ];then            echo -e $mesg;            exit;          fi;        done;     done < $file ;     echo -e "Well, congratulations!! You fixed my conflict!!\nIf you would like to continue, then you should checkout to the $(echo 90mP8ouQHsNe | tr -d '0-9A-Z') branch!!\n" ;    else       echo -e $mesg;       exit;    fi;  else    echo "Looks like you passed in the wrong file"; fi
   12  #!/bin/bash
   13  if [ -z $1 ]; then    echo "well, someone didn't want to run the script with a file...";   exit; fi
   14  file=$1
   15  bug=7c85d987a917c2a555d1391426978f05
   16  mesg="Level 7: \n Linus has been here...\nI love messing with these amateur programmers!!\nIf you want some real fun, then you should try resolving a conflict between this branch (tree) and code4life.\nI introduced a little bug that you should fix in the conflict. >:)\nAfter you merge these 2 files you should run the shell script again!!\n\nGood Luck!!!\n\n Hint: https://help.github.com/articles/resolving-a-merge-conflict-from-the-command-line/ "
   17  merges=$(git log --format=%h --merges | head -1)
   18  csum="md5sum"
   19  if [ $(echo "$OSTYPE" | grep darwin) ];then     csum="md5"; fi
   20  if [ "$file" = "nextclue_input.cpp" ];then    if [ ${merges} ]; then      while read p; do        for w in $p;do          if [ `echo $w | $csum | awk '{print $1}'` = $bug ];then            echo -e $mesg;            exit;          fi;        done;     done < $file ;     echo -e "Well, congratulations!! You fixed my conflict!!\nIf you would like to continue, then you should checkout to the $(echo 90mP8ouQHsNe | tr -d '0-9A-Z') branch!!\n" ;    else       echo -e $mesg;       exit;    fi;  else    echo "Looks like you passed in the wrong file"; fi
   21  git status
   22  git commit -m "git game 1st commit"
   23  git push
   24  git checkout mouse
   25  cat README.md
   26   git diff mouse bug -- remember.
   27  git diff mouse bug --remember
   28  git diff mouse bug -- remember
   29  git checkout Henry
   30  ls
   31  cat README.md
   32  git tag -d
   33  git checkout Henry
   34  cat README.md
   35  git tag
   36  git tag -d
   37  git checkout mouse
   38  git tag
   39  git tag -d
   40  git tag
   41  git tag Henry
   42  git tag -d Henry
   43  git tag
   44  git checkout Henry
   45  cat README.md
   46  git remote -v
   47  git remote add upstream  https://github.com/Liona-geb/HtH-gitgame.git
   48  git remote -v
   49  git remote add upstream  https://github.com/drami025/git-game.git
   50  git remote add drami https://github.com/drami025/git-game.git
   51  git remote v
   52  git remote -v
   53  git checkout master
   54  git pull drami master
   55  cat README.md
   56  history 100 > gitHistory.md
