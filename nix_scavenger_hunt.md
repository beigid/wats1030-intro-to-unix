# *nix Scavenger Hunt

Complete the following challenges using the command-line interface on your favorite
Unix or Linux operating system. You are welcome and encouraged to consult any
additional documentation online or in books.

Please add your answers/responses/text pastes to the document after each prompt.

Note: For some of the challenges you will need to reference files included with
this repository, so you will need to fork the repo into your own Github account
and then clone it to your development environment.

## The Challenges

### Navigating the Filesystem

* Get an idea of where you are in the operating system. Use the `pwd` command to find your "path to working directory"--your current location in the filesystem of your devbox. *Paste the output of the `pwd` command here:*

```
/home/cabox/workspace
```

* Discover more about this filesystem. Use `ls` (the "list" command)to see what is in this directory. *What directories and files do you see when you run `ls`?*

**1. README.md  
1. challenge_files  
1. nix_scavenger_hunt.md  
1. nix_scavenger_hunt_stretch.md
1. challenge_files  
1. super_scavengers.md
1. LICENSE**

* You can use *options* to modify how a command runs. Try using `ls -alh` to see the contents of your current directory. *How are the results different when you use the `-alh` options?*

```
drwxrwxr-x  4 cabox cabox 4.0K Jan 17 23:30 .
drwxr-xr-x 10 cabox cabox 4.0K Jan 18 00:07 ..
drwxrwxr-x  8 cabox cabox 4.0K Jan 18 00:19 .git
-rw-rw-r--  1 cabox cabox 1.1K Jan 17 23:30 LICENSE-rw-rw-r--  1 cabox cabox 2.7K Jan 17 23:30 README.md
drwxrwxr-x  7 cabox cabox 4.0K Jan 17 23:30 challenge_files
-rw-rw-r--  1 cabox cabox 5.6K Jan 18 00:20 nix_scavenger
_hunt.md
-rw-rw-r--  1 cabox cabox  317 Jan 17 23:30 nix_scavenger
_hunt_stretch.md-rw-rw-r--  1 cabox cabox  191 Jan 17 23:30 super_scaveng
ers.md
```

* The `man` ("manual") command tells you more about how any given command works. (*WARNING:* CodeAnywhere does not support the man command. You can click the following link to complete this task: http://linux.die.net/man/). Run `man` to see instructions about how to use `man`. Then use `man` to learn what the `a`, `l`, and `h` options mean when used with the `ls` command. *Write down what those options do?*

```
-a, --all
      do not ignore entries starting with .
-l
use a long listing format

-h, --human-readable
with -l, print sizes in human readable format (e.g., 1K 234M 2G)

```

* Commands can also take *arguments*, which are usually the names of files or locations that you want the command to work with. Try running `ls /` to see what files are in the *root* directory of the filesystem. *What files and directories do you see listed?*


1. bin  
1. boot  
1. dev  
1. etc  
1. home  
1. lib  
1. lib64  
1. media  
1. mnt  
1. opt  
1. proc  
1. root  
1. sbin  
1. selinux  
1. srv  
1. sys  
1. tmp  
1. usr  
1. var

* A Unix filesystem has a few special shortcuts to refer to specific locations. `/` indicates the *root* of the filesystem, meaning the top-most directory in the filesystem hierarchy. Use the `cd` ("change directory") command to move to the root directory. (Hint: Use `man` to look up the `cd` command if you have any issues) *Then run `pwd` and paste the output here:*

```
/home/cabox
```

* Another special shortcut in Unix is the `~` location. This indicates the *user root* directory, meaning the top-most directory in the hierarchy that comes below your user account. Use `cd` to move to `~`. *Run `pwd` and paste the response here:*

```
/home/cabox
```

* Change directory into the `challenge_files` directory. Use `ls` to find only the files with a `.demo` pattern. *How many files do you find?*

```
01                       Hillard-Ziemann.user
2015_special_stuff.demo  Isadora-Leffler.user
Afton-Jast.user          Jaxen-Gleichner.user
Aimee-Maggio.user        Jayme-Rodriguez.user
Alfonso-Gottlieb.user    Jenni-O'Connell.user
Allen-Kemmer.user        Johny-Borer.user
Almina-Cormier.user      Kassandra-Barrows.user
Alta-Lemke.user          Keely-Hilpert.user
Amina-McGlynn.user       Kenyatta-Hickle.user
Anabel-Hammes.user       Kiana-Kulas.user
Ancel-Conn.user          Kirstin-Hoppe.user
Anjali-Halvorson.user    Kwame-Schmitt.user
Ardath-Kuvalis.user      Ladonna-Lueilwitz.user
Avah-Dickinson.user      Lala-Will.user
Ayaan-Stiedemann.user    Leia-Hudson.user
Aylin-Grant.user         Leia-Ziemann.user
Bedford-Sipes.user       Lillard-Purdy.user
Benita-King.user         Lilly-Kohler.user
Benito-Stoltenberg.user  Lissie-Strosin.user
Beverlee-Moen.user       Mannie-Ritchie.user
Brad-Thiel.user          Masako-Lind.user
Brayan-Douglas.user      Melisa-Yundt.user
Bria-Satterfield.user    Michelina-Kuphal.user
Bridgette-Reichel.user   Minnie-Jacobi.user
Britt-Erdman.user        Murdock-Leffler.user
Britta-Hammes.user       Mychal-Corkery.user
Bryant-Kuhic.user        Nakita-Nader.user
Bryton-Aufderhar.user    Nayely-Dare.user
Caitlin-Grady.user       Nicholas-Strosin.user
Carroll-Hartmann.user    Niles-Runte.user
Claudie-McClure.user     Nina-Sporer.user
Clemente-Haley.user      Noreta-Steuber.user
Cleo-VonRueden.user      Ovid-Bogan.user
Codie-Romaguera.user     Randell-Sauer.user
Cooper-Reynolds.user     Remy-Renner.user
Corrie-Bogisich.user     Ronna-Hermann.user
Dannielle-Green.user     Rosalind-Wisozk.user
Deedee-Jacobson.user     Rosena-Simonis.user
Desiree-Marks.user       Sandie-Balistreri.user
Deven-Rutherford.user    Sharen-Hansen.user
Doyle-Jones.user         Sherrill-Russel.user
Dustyn-O'Connell.user    Sherwin-Kovacek.user
Elza-Mraz.user           Sherwood-Rath.user
Emory-Crona.user         Shyheim-Murazik.user
Erin-Walker.user         Siobhan-Kirlin.user
Estela-Schultz.user      Tomas-Kutch.user
Fernanda-Tromp.user      cloaked-wookie.demo
Fletcher-Rice.user       credit_cards.txt
Fred-Ryan.user           credit_cards2.txt
Genie-Abshire.user       scooter-double-mamba.demo
Grace-Tromp.user         serial-numbers
Grant-Cronin.user        test2
Hali-Roob.user           tmp
Harland-Schoen.user      wow
Harrell-Quitzon.user
```

* Use the `cd` command to move "up" one directory. *Where are you in the filesystem now?*

```
/home/cabox/workspace
```

* Press the up arrow on your keyboard. *What just happened?*

```
cd ../ The last command I typed in!
```

* Press the up arrow a few more times. *What do you see?*

```
The last few commands I had typed into the SSH terminal.
```

* Run the `history` command. *What do you see?*

```
    1  pwd
    2  git status
    3  git add .
    4  git commit -m "started working on challenges"
    5  git push -u origin gh-pages:gh-pages
    6  git push -u origin gh-pages
    7  git status
    8  git push git checkout -b gh-pages
    9  git status
   10  git checkout -b gh-pages
   11  git status
   12  git push -u origin gh-pages:gh-pages
   13  clear
   14  ls
   15  git status
   16  git commit -m "Worked on creating a list"
   17  git add .
   18  git commit -m "worked on creating a list for second answers"
   19  git push
   20  clear
   21  ls-ah
   22  ls -alh
   23  -alh
   24  man
   25  uname -a
   26  date
   27  ls
   28  -S
   29  S
   30  -S
   31  -a
   32  cmd < file
   33  clear
   34  who
   35  history
   36  fortune
   37  gimp
   38  df
   39  passwd
   40  mail
   41  ps <opt>
   42  cd Documents
   43  cd dirname
   44  pwd
   45  cd
   46  lynx
   47  rlogin
   48  cal
   49  whoami
   50  finger
   51  ps -u cabox
   52  clear
   53  ls /
   54  cd
   55  /
   56  cd
   57  /
   58  pwd
   59  ~
   60  pwd
   61  ~
   62  cd
   63  ~
   64  pwd
   65  challenge_files
   66  /challenge_files
   67  cd
   68  ~
   69  cd
   70  ls
   71  /
   72  .
   73  ..
   74  .
   75  cd
   76  /cd
   77  cd/
   78  /challenge_files
   79  cd
   80  ~
   81  "cwd": "~/workspace",
   82  ~/
   83  ~/challenge_files
   84  cwd
   85  "cwd"
   86  pwd
   87  ls ~
   88  cd ~
   89  pwd
   90  cd workspace
   91  cd challenge_files
   92  pwd
   93  ls
   94  cd ../
   95  pwd
   96  cd challenge_files
   97  pwd
   98  cd
   99  pwd
  100  cd challenge_files
  101  pwd
  102  cd
  103  pwd
  104  cd workspace
  105  cd challenge_files
  106  pwd
  107  cd
  108  pwd
  109  cd workspace
  110  cd challenge_files
  111  pwd
  112  cd ../
  113*
  114  history
```
### Observing the System

* Discover what account you are logged into using the `whoami` command. *What username are you currently using?*

```
cabox
```

* Discover who else is on your system with the `who` command. *Are any other users using your system? If so, list them here:*

```
cabox    pts/0        Jan 18 21:12 (52.161.27.120)
```
* How long has your system been running? Use `uptime` to see, and *paste the result here:*

```
21:29:40 up 17 min,  1 user,  load average: 0.00, 0.00, 0.00
```
* Run `ps aux` and review the results. (Hint: Use `man` to learn more about the `ps` command and options.) *How do you interpret what you see here?*

```
I interpret what I see here as all the running processes currently, their statuses, and their resource usages (CPU, MEM, etc.)
```
* Run `top` and review the results. (Hint: You may need to use `ctrl-c` to get out of this app.) *How do you interpret what you see here?*

```
This command appears to produce an ordered list of running processes. It also appears to be active and refreshing or updating frequently
```

### Finding and Viewing Files

* Make sure you are in the `challenge_files` directory. Use the `*` wildcard to find all the files that have the word "credit" in the filename. *How many files did you find?*

```
credit_cards.txt
credit_cards2.txt
```
* Use the `more` command to view one of the `credit_cards` files you just discovered. (Hint: Type `q` to quit viewing the file. Press the `spacebar` to page down. Use your keyboard arrows to move up/down.) *What is the date in the file you have viewed?*

```
credit_card.txt Last updated: 01-15-2015
```
* Use the `find` command to search for files more effectively. Search the sub-directories under `challenge_files` to find the location of the file named `modi_laboriosam.txt`. *Where is that file located?*

```
./tmp/modi_laboriosam.txt
```

* Use the `grep` command to search for text within a file. Use `grep` on all the `.user` files in `challenge_files` to find which files contain "WA" (the abbreviation for Washington state). *How many files did you find?*

```
Britt-Erdman.user:O'Harachester, WA 37261
Lissie-Strosin.user:Jewessfurt, WA 00816-7241
```

* Use the `-r` option of `grep` to *recursively* find the text "Waldo" hidden in a file somewhere under the `challenge_files` directory. *Paste the result showing the file and line where the word "Waldo" shows up.*

```
serial-numbers/eaque_molestiae.txt:Ut est maiores quia autem. Nisi modi Waldo sed corporis sit explicabo ut est. Et est placeat ea sunt sunt consectetur sunt incidunt. Explicabo vel esse blanditiis dolorem culpa non quia.

```

### Pipes and Connecting Commands

* Sometimes it's useful to output the results of a command to a text file for further analysis, reference, or processing. Try running `ls > files.txt`. Notice that the file `files.txt` was created. View that file using `more`. *What do you see in the `files.txt` file?*

```
01
2015_special_stuff.demo
Afton-Jast.user
Aimee-Maggio.user
Alfonso-Gottlieb.user
Allen-Kemmer.user
Almina-Cormier.user
Alta-Lemke.user
Amina-McGlynn.user
Anabel-Hammes.user
Ancel-Conn.user
Anjali-Halvorson.user
Ardath-Kuvalis.user
Avah-Dickinson.user
Ayaan-Stiedemann.user
Aylin-Grant.user
Bedford-Sipes.user
Benita-King.user
Benito-Stoltenberg.user
Beverlee-Moen.user
Brad-Thiel.user
Brayan-Douglas.user
Bria-Satterfield.user
Bridgette-Reichel.user
Britt-Erdman.user
Britta-Hammes.user
Bryant-Kuhic.user
Bryton-Aufderhar.user
Caitlin-Grady.user
Carroll-Hartmann.user
Claudie-McClure.user
Clemente-Haley.user
Cleo-VonRueden.user
Codie-Romaguera.user
Cooper-Reynolds.user
Corrie-Bogisich.user
Dannielle-Green.user
Deedee-Jacobson.user
Desiree-Marks.user
Deven-Rutherford.user
Doyle-Jones.user
Dustyn-O'Connell.user
Elza-Mraz.user
Emory-Crona.user
Erin-Walker.user
Estela-Schultz.user
Fernanda-Tromp.user
Fletcher-Rice.user
Fred-Ryan.user
Genie-Abshire.user
Grace-Tromp.user
Grant-Cronin.user
Hali-Roob.user
Harland-Schoen.user
Harrell-Quitzon.user
Hillard-Ziemann.user
Isadora-Leffler.user
Jaxen-Gleichner.user
Jayme-Rodriguez.user
Jenni-O'Connell.user
Johny-Borer.user
Kassandra-Barrows.user
Keely-Hilpert.user
Kenyatta-Hickle.user
Kiana-Kulas.user
Kirstin-Hoppe.user
Kwame-Schmitt.user
Ladonna-Lueilwitz.user
Lala-Will.user
Leia-Hudson.user
Leia-Ziemann.user
Lillard-Purdy.user
Lilly-Kohler.user
Lissie-Strosin.user
Mannie-Ritchie.user
Masako-Lind.user
Melisa-Yundt.user
Michelina-Kuphal.user
Minnie-Jacobi.user
Murdock-Leffler.user
Mychal-Corkery.user
Nakita-Nader.user
Nayely-Dare.user
Nicholas-Strosin.user
Niles-Runte.user
Nina-Sporer.user
Noreta-Steuber.user
Ovid-Bogan.user
Randell-Sauer.user
Remy-Renner.user
Ronna-Hermann.user
Rosalind-Wisozk.user
Rosena-Simonis.user
Sandie-Balistreri.user
Sharen-Hansen.user
Sherrill-Russel.user
Sherwin-Kovacek.user
Sherwood-Rath.user
Shyheim-Murazik.user
Siobhan-Kirlin.user
Tomas-Kutch.user
cloaked-wookie.demo
credit_cards.txt
credit_cards2.txt
files.txt
scooter-double-mamba.demo
serial-numbers
test2
tmp
wow

```

* Notice that if you run `ls -alh` in the `challenge_files` directory, the files scroll by very quickly. Sometimes it would be better to get the results in a paginated format. Try running `ls -alh | more`. *Describe what you see when you run `ls -alh | more`.*

```
total 460K
drwxrwxr-x 7 cabox cabox 4.0K Jan 19 17:41 .
drwxrwxr-x 4 cabox cabox 4.0K Jan 19 17:23 ..
drwxrwxr-x 2 cabox cabox 4.0K Jan 19 17:13 01
-rw-rw-r-- 1 cabox cabox    0 Jan 19 17:13 2015_special_stuff.demo
-rw-rw-r-- 1 cabox cabox   93 Jan 19 17:13 Afton-Jast.user
-rw-rw-r-- 1 cabox cabox   85 Jan 19 17:13 Aimee-Maggio.user
-rw-rw-r-- 1 cabox cabox   79 Jan 19 17:13 Alfonso-Gottlieb.user
-rw-rw-r-- 1 cabox cabox  100 Jan 19 17:13 Allen-Kemmer.user
-rw-rw-r-- 1 cabox cabox   86 Jan 19 17:13 Almina-Cormier.user
-rw-rw-r-- 1 cabox cabox   87 Jan 19 17:13 Alta-Lemke.user
-rw-rw-r-- 1 cabox cabox   79 Jan 19 17:13 Amina-McGlynn.user
-rw-rw-r-- 1 cabox cabox   78 Jan 19 17:13 Anabel-Hammes.user
-rw-rw-r-- 1 cabox cabox   61 Jan 19 17:13 Ancel-Conn.user
-rw-rw-r-- 1 cabox cabox   87 Jan 19 17:13 Anjali-Halvorson.user
-rw-rw-r-- 1 cabox cabox   64 Jan 19 17:13 Ardath-Kuvalis.user
-rw-rw-r-- 1 cabox cabox   90 Jan 19 17:13 Avah-Dickinson.user
-rw-rw-r-- 1 cabox cabox   79 Jan 19 17:13 Ayaan-Stiedemann.user
-rw-rw-r-- 1 cabox cabox   79 Jan 19 17:13 Aylin-Grant.user
-rw-rw-r-- 1 cabox cabox   70 Jan 19 17:13 Bedford-Sipes.user
-rw-rw-r-- 1 cabox cabox   82 Jan 19 17:13 Benita-King.user
-rw-rw-r-- 1 cabox cabox   92 Jan 19 17:13 Benito-Stoltenberg.user
-rw-rw-r-- 1 cabox cabox   83 Jan 19 17:13 Beverlee-Moen.user
-rw-rw-r-- 1 cabox cabox   76 Jan 19 17:13 Brad-Thiel.user
-rw-rw-r-- 1 cabox cabox   68 Jan 19 17:13 Brayan-Douglas.user
-rw-rw-r-- 1 cabox cabox   80 Jan 19 17:13 Bria-Satterfield.user
-rw-rw-r-- 1 cabox cabox   70 Jan 19 17:13 Bridgette-Reichel.user
-rw-rw-r-- 1 cabox cabox   78 Jan 19 17:13 Britt-Erdman.user
-rw-rw-r-- 1 cabox cabox   66 Jan 19 17:13 Britta-Hammes.user
-rw-rw-r-- 1 cabox cabox   68 Jan 19 17:13 Bryant-Kuhic.user
-rw-rw-r-- 1 cabox cabox   86 Jan 19 17:13 Bryton-Aufderhar.user
-rw-rw-r-- 1 cabox cabox   82 Jan 19 17:13 Caitlin-Grady.user
-rw-rw-r-- 1 cabox cabox   99 Jan 19 17:13 Carroll-Hartmann.user
-rw-rw-r-- 1 cabox cabox   80 Jan 19 17:13 Claudie-McClure.user
--More--
```

* Earlier, when you viewed the list of active processes on your devbox using `ps aux`, the list was probably really long. You can make this list more manageable by using the pipe (`|`) to filter the results of `ps` using `grep`. Run `ps aux | grep <your_username>` to see what processes are running for your specific user. *Paste the list of processes that reference your username here:*
```
root       524  0.0  0.6  63876  3328 ?        Ss   17:25   0:00 sshd: cabox [priv]
cabox      526  0.0  0.2  64008  1508 ?        S    17:25   0:00 sshd: cabox@notty
cabox      527  0.0  0.1  12860  1016 ?        Ss   17:25   0:00 /usr/lib/openssh/sftp-server
root       528  0.0  0.6  63876  3480 ?        Ss   17:28   0:00 sshd: cabox [priv]
cabox      530  0.0  0.2  63876  1464 ?        S    17:28   0:00 sshd: cabox@pts/0
cabox      531  0.0  0.8  20564  4484 pts/0    Ss   17:28   0:00 -bash
cabox      742  0.0  0.2  15520  1140 pts/0    R+   17:46   0:00 ps aux
cabox      743  0.0  0.1   8816   764 pts/0    S+   17:46   0:00 grep --color=auto cabox
```
