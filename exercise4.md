    1  ls
    2  pwd
    3  cd test
    4  ls
    5  cd ..
    6  mkdir test2
    7  ls
    8  cd test2
    9  nano newfile.md
   10  ls
   11  cd ..
   12  pwd
   13  wget https://github.com/jgm/pandoc/releases/download/1.19.2.1/pandoc-1.19.2.1-1-amd64.deb
   14  sudo dpkg -i pandoc-1.19.2.1-1-amd64.deb
   15  pandoc -v
   16  history
   17  history > dhbox-work-today.md
   18  ls
   19  clear
   20  ls
   21  nano dhbox-work-today.md
   22  clear
   23  ls
   24  mkdir ex4
   25  cd ex4
   26  pwd
   27  ls
   28  nano readme.md
   29  git init
   30  ls
   31  git status
   32  git add -A
   33  git status
   34  git commit -m "first commit woohoo"
   35  nano anotherfile.md
   36  nano yetanotheerfile.md
   37  git status
   38  git add -A
   39  git status
   40  git commit -m "second dummy files"
   41  touch data.csv
   42  touch data2.csv
   43  ls
   44  git add -A
   45  git status
   46  git commit -m "third csv"
   47  git log
   48  git checkout -b experiment c91c40ae3d4f9a05ed1d70cec17e97c8ec65fc93
   49  ls
   50  nano experimentalfile.md
   51  git add -A
   52  git commit -m "experiment1"
   53  ls
   54  git checkout master
   55  git merge master experiment
   56  clear
   57  git status
   58  ls
   59  history
   60  history > exercise4.md
