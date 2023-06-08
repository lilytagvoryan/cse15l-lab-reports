# Doing it All From the Command Line
## These steps involve editing, compiling, and running commands from the terminal!
### 1. Log into ieng6
Begin by logging into your ieng6 account by entering ```ssh cs15lsp23[!!]@ieng6.ucsd.edu``` ```<enter>``` into the terminal under ```bash```. Subsitute the ```!!``` for the letters you recieved for your *own* ieng6 account. After entering, ```Password:``` should pop up which in turn will permit the user (you) to enter their/your password. It should look something similar to the image below.

<img width="933" alt="image" src="https://github.com/lilytagvoryan/cse15l-lab-reports/assets/123005863/bd5dc119-94f8-4f1a-a4c0-d8acffe9b862">

***

### 2. Clone your fork of the repository from your Github account
Next, you must clone your fork of the repository through your account on Github. You do this by inputting ```git clone https://github.com/ucsd-cse15l-s23/lab7``` ```<enter>``` within the terminal. The output is shown below.

<img width="689" alt="image" src="https://github.com/lilytagvoryan/cse15l-lab-reports/assets/123005863/299ebee1-a889-4877-9811-4a1c15a6b3da">

***

### 3. Run the tests, demonstrating that they fail
You can run the tests by first typing ```ls``` to see all the folders/files you can move into. Then, type ```cd lab7``` to move into that directory and ```ls``` to see what is in that folder. Type ```bash test.sh``` to run whatever is in that file right after checking to see that ```test.sh``` exists (from the previous ```ls``` command). The steps are also shown in image below.

*Note: press```<enter>```after each command.*

<img width="715" alt="image" src="https://github.com/lilytagvoryan/cse15l-lab-reports/assets/123005863/f5ef8e27-c63a-46b4-b368-b5f209991a0e">

***

### 4. Edit the code file to fix the failing test
You can view the code file by entering ```vim ListExamples.java```. Then, begin editing the file to fix the appearing failing test. You can edit the code by inserting ```/.add<enter><n><n><n><n><j><j><x><i><2><esc>:wq<enter>```. This should not only allow you to edit the text but save it as well. 

The ```/.add``` searches for anything after the slash, in this case ```.add```. The user then must press ```<enter>```. Next, with just 4 clicks of ```<n>``` (for **next** character(s) searched) and 2 clicks of ```<j>``` (to move down a line(s)), you're brought to the line you must make your edit. The ```<x>``` removes a character, the ```<i>``` puts the user in **insert** mode, and the ```<2>``` replaces the existing ```1``` in order to fix the bug. The ```<esc>``` takes the user out of insert mode and into normal mode, and ```:wq``` finally allows the user to save and quit the file. The user concludes by pressing ```<enter>```. 

<img width="752" alt="image" src="https://github.com/lilytagvoryan/cse15l-lab-reports/assets/123005863/5c6793b4-56aa-47ee-b2f7-eba371598b08">

***

### 5. Run the tests, demonstrating that they now succeed
You can run these tests to see if they now work by using the terminal. You do this by pressing ```<up><up>``` (indicating the up arrows) where you should see ```bash test.sh``` in order to rerun the tests. You can then press ```<enter>``` to see your results as shown below.

<img width="537" alt="image" src="https://github.com/lilytagvoryan/cse15l-lab-reports/assets/123005863/9fde7444-c6e3-494e-a0a5-039efbb8c162">

***

### 6. Commit and push the resulting change to your Github account (you can pick any commit message!)
You can finally commit by entering ```git add ListExamples.java``` ```<enter>``` to add the file onto the next commit. Then, ```git commit``` ```<enter>```. After this you'll be shown a screen similar to the one below where you'll write your commit message. I used "Committed!" I pressed ```<esc>``` right after go into normal mode. I then typed ```:wq``` in order to save and quit.

<img width="557" alt="image" src="https://github.com/lilytagvoryan/cse15l-lab-reports/assets/123005863/691ddce3-b96a-4793-af89-a577060a5790">

<img width="566" alt="image" src="https://github.com/lilytagvoryan/cse15l-lab-reports/assets/123005863/2f49516a-48d8-4c09-9b6b-aa2079af7dfa">

After, you can type ```git push``` ```<enter>``` to push all changes you have made to your committed repository. 



