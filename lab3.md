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
  What this command did was print the number of lines where "health" showed up in the text file within biomed. 
  ```
  grep -c "report" technical/government/Alcohol_Problems/Session2-PDF.txt
  ``` 
  ```
  13
  ```
  This command printed the number of lines where "report" was present in the Session2 text file of Alcohol_Problems.

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
 This command printed the searched lines and two lines before and after the matches of "death" in the text file in plos.
 

***

#### 3. command
  * h
  * h

***

#### 4. command
  * h
  * h
