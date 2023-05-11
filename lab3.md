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
 What this command did was print the number of lines where "health" showed up in the text file within biomed. This is useful because if you want to use it on several articles, for instance, you may easily pick and choose the one that has a higher count of the word you're looking for (medical, in this example) to see if there is any additional information on it.
  ```
  grep -c "report" technical/government/Alcohol_Problems/Session2-PDF.txt
  ``` 
  ```
  13
  ```
 This command printed the number of lines where "report" was present in the Session2 text file of Alcohol_Problems. This command was helpful for this search since it allows you to find any specific information on a "report" for that specific session.

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
 
This command looked through the file and printed two lines before and after the matches of "death" in the text file within plos. With this command, you're able to read any information about "death," but also look at any sentences before and after it for additional context.


```
grep -C 1 "medical" technical/biomed/1471-2334-1-10.txt
```

```
three villages of each PHC during autumn season
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

This command searched the file and printed one line before and after the matches of "medical" in the text file within biomed. This command allows the user to look at information where "medical" is specifically stated with lines of text on it, before and after.

***

#### 3. ```grep "[text]$"```

```
grep "ls$" technical/911report/chapter-5.txt 
```

```
                petition was pending, Binalshibh lived in Hamburg and associated with individuals
```
What this command searched for was the line(s) ending in "ls" as written with the "$" to indicate the end of the search. It printed the line ending in "ls" within a text file in 911report that permits the user to find the specific area where the ending of the word may be.
```
grep "ce$" technical/government/About_LSC/Progress_report.txt 
```
```
Wood) and Pat Hanrahan and Wendy Burnette in the Executive Office
In March of 2001, LSC released Building State Justice
In April, LSC announced significant changes in service
experience in LSC-funded programs. Many staff also have experience
part-time consultants. Their combined expertise includes resource
A TIG conference was held in Chicago in October to introduce
ensure that each web site supports the entire state justice
application process took place at the National Equal Justice
State Justice Institute, the Open Society Institute and Justice
Courts and the Horowitz Foundation) on building broader justice
discuss the preparation of this manual at the TIG 2001 conference
reviews, published as a "Program Review Guide." It is a reference
Commitment: Undertake a series of program evaluation performance
The Creation of Efforts to Link with the International Justice
Addressing the Pan Pacific Legal Aid Conference
directors, or clients. There was also a two-day national conference
Meaningful Access to Justice
North Carolina and Arkansas held their first Equal Justice
The Supreme Court of Washington created a new Task Force
```
This command looked for and printed the line(s) that ended with "ce" as followed by the "$" in the text file. This search is helpful since it allows the user to search for the specific ending of "ce" of words within the file, which can be useful if you're only looking for the ending of those words.
***

#### 4. ```grep -v```
```
grep -v "a" technical/biomed/1471-2369-3-6.txt    
```
```
 Methods
        
          Cell culture
          B, 1 μg/ml hydrocortisone, 10 μg/ml insulin, 5.5 mg/ml
          Growth Supplement (PerImmune, Rockville, MD) + 100 U/ml
        
        
          nm.
          nm.
        
        
        
      
      
        Results
        Stx-1 (72 hr exposure to toxin) dose-dependently killed
        fM).
        dose-response from 10 -5- 10 -11g/L Stx-1, in ten-fold
      
      
        Stx-producing 
        effect of sex steroids on Stx responsiveness, however, the
        previous studies, within the limits of the cell culture
        Cells were exposed to the steroids for up to one week in
        E. coli 0157:H7 [ 14 ] . Further,
        to be responsive to sex steroids (e.g.
        determined.
      
      
        HUS hemolytic-uremic syndrome
      
      
        Competing interests
      
      
        Authors' Contributions
        the experiments.
 ```
This command looked up all the lines where "a" does NOT show up. Contrasting from the other commands, -v looks for the places where the given string is NOT shown which is helpful if you want to find information that does not show up in the article you are viewing.
```
grep -v 'a\|e\|i' technical/plos/pmed.0010028.txt     
```
```
count of 3.0 × 10
        
        
        
        
          
          
          
          
          
          
        
        
        
        
          
          
          
          
          
          
        
        
        
        
        
      
      
        
        
        
        
        
        
        
        
      
      
        10
```
This command printed all the lines where "a", "e", nor "i" showed up in. Therefore, not a lot of text appeared since those vowels were constantly used throughout the text file in plos; this is helpful if you're trying to find analytics on data without getting whole words.

***
*The cite I saw these commands from was [https://www.geeksforgeeks.org/grep-command-in-unixlinux/](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)*
