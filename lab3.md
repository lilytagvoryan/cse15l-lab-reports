# Researching Commands
The ```grep``` command consists of multiple alternatives or command-like options used to search through files for a given string. Here are some of the ways it's used... 

***

#### 1. ```grep c-```
  ```
  grep -c "health" technical/biomed/1472-6963-3-7.txt
  ```
  ```
  26
  ```
 * What this command did was print the number of lines where "health" showed up in the text file within biomed. 
  ```
  grep -c "report" technical/government/Alcohol_Problems/Session2-PDF.txt
  ``` 
  ```
  13
  ```
 * This command printed the number of lines where "report" was present in the Session2 text file of Alcohol_Problems.

***

#### 2. ```grep -C[NumberOfLines(n)] [search] [file]``` 
  ```
  grep -C 2 "death" technical/plos/pmed.0020060.txt
  ``` 
  
  ```
  Preparing for Death
        How does one prepare for death? Those who have created a public persona must add to any
        spiritual ponderings about eternity the mundane chore of organizing their literary archives
        to protect any of life's secrets that seem worth the effort. That task involves choosing
--
        published volumes of carefully edited literary diaries. When someone at a seminar remarked
        to her that her life seemed more, well, racy than those diaries revealed, she smiled
        mysteriously and said that after the death of all concerned, “unexpurgated” editions would
        be published. Several decades later, companion volumes to the literary diaries revealed
        passionate incest with her father, Joachim Nin, an affair with her analyst, Otto Rank, and
--
        no-longer-swimming fish below the earth from that of grown-up exhumers? Consider Gira
        Fornaciari, who unearthed 49 members of the Medici family to confirm various causes of
        death, or the committee that had Beethoven and Schubert dug up to transfer them to more
        secure zinc coffins (borrowing both heads for a bit more measuring, and swiping Schubert's
        luxuriant, larvae-laden hair while they were at it). Archaeologists have braved curses and
 ```
* This command looked through the file and printed two lines before and after the matches of "death" in the text file within plos.
```
grep -C 1 "medical" technical/biomed/1471-2334-1-10.txt
```
```three villages of each PHC during autumn season
          (December, 1999), by one medical specialist by
          establishing a mobile field clinic after obtaining
--
        splenomegaly was observed as recorded elsewhere [ 18 19 ] .
        However, it requires the services of a medical specialist
        who is not certain whether the spleen is entirely due to
--
        diagnosis, which would overcome the usual delay associated
        with dependence on medical laboratories. Thus rapid test
        could be a better diagnostic method in 
 ```
* This command searched the file and printed one line before and after the matches of "medical" in the text file within biomed.
***

#### 3. ```grep "[text]$"```
```
grep "ls$" technical/911report/chapter-5.txt 
```
```
                petition was pending, Binalshibh lived in Hamburg and associated with individuals
```
* What this command searched for was the line(s) ending in "ls" as written with the "$" to indicate the end of the search. It printed the line ending in "ls" within a text file in 911report.

***

#### 4. command
  * h
  * h
