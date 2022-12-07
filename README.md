
<h1>Welcome to HANGMAN</h1>

This is a Python terminal version of [Hangman](https://forgottenit-hangman.herokuapp.com). It runs in the Code Institute mock terminal. 

The User is given a certain amount of attempts to try guess letters in a hidden word picked by the computer.

You can read more about Hangman on [Wikipedia](https://en.wikipedia.org/wiki/Hangman_(game))

## How to Play

* At the Loading screen the User is asked to press Enter, then thr rules are displayed
* The user is asked to choose a category, these are either : Words, Songs (Singles), Films, Books or Countries. Or the user can let the computer pick the category.
* The user is then shown the background story for their category. The user then decides if they want to play Easy (10 lives), Medium (8 lives) or Hard (6 lives)
* The Computer picks a word from the chosen category and displays blanks (_'s) to the user to signify the amount of letters in the word. If the word contains symbols such as hyphens or numbers (1,2,3 etc.) These are displayed to the user. If it's roman numerals (i.e. I or V etc.) These are not displayed. 
* The User is then asked to try guess a letter that is in the word. The input will only allow lettera to be attempted. It also will tell the user if they've already attempted the letter.
* If the User's guess is in the word, the computer displays the letter (or letters if there are multiple instances of the letter) in place of the blanks. If it is not in the word, the user loses a life.
* The User keeps guessing until they have guessed all the correct letters (They win) or runs out of lives/attempts (They lose)
* After the game they are shown the corresponding End story, and asked if they want to play again, if they enter "Y" the game reverts back to the category choice, any other input leads back to the intro image

## Flow Chart for Hangman

<img src="Docs/Flowchart.png">

## Technology used

1. GitPod for writing the code
2. Python as the programming language
3. Heroku for deployment
4. Code Instistute Terminal for displaying finished product

## Testing



## Constraints

* The deployment terminal is set to 80 columns by 24 rows. That means that each line of text needs to be 80 characters or less otherwise it will be wrapped onto a second line.
* A "\n" symbol had to be inserted at the end if user input print outs due to a quirk in the terminal interface.

## Deployment
<h3>GitPod<h3>

* To deploy in GitPod load from the GitHub repository, then enter "Python3 run.py" in the main terminal

<h3>Heroku</h3>
1. Go to the Heroku Dashboard and Click "New" in the top right corner then click "Create new app"

  <img src="Docs/Home.png">

2. Name the App and set the region to Europe

  <img src="Docs/App%20Information.png">

3. Go to Settings and, Click Reveal Config Vars and set keys to PORT and value to 8000

  <img src="Docs/VARS.png">

4. Click Add Buildpacks, add Python, save changes.

  <img src="Docs/Buildpacks1.png">

  <img src="Docs/Buildpacks2.png">

5. Repeat step 4, but this time add Node.js, once completed it should look like below, with heroku/python above herokue/node.js, if now they can be clicked upon and dragged to change to this order.

  <img src="Docs/Completed%20Buildpacks.png">

6. Navigate to the Deploy section. Select GitHub from the Deployment Method section, connnect your GitHub Repo by selecting the repo name (in this case, hangman) and Authorise when prompted.

  <img src="Docs/Deploy%20menu.png">

  <img src="Docs/Deployment%20Method.png">

  <img src="Docs/Connect%20to%20Github.png">

7. Click Enable Automatic Deploys. Once Changes are pushed to your repo, the app will be constucted.

  <img src="Docs/Automatic%20Deploys.png">

8. Finally, click Open App to run the App in the Code Institute Terminal

  <img src="Docs/Open%20App.png">

## Acknowledgements 
* https://wtools.io/convert-list-to-json-array for converting lists to json format
* https://www.britannica.com/topic/list-of-countries-1993160 for list of countries
* https://www.theguardian.com/news/datablog/2012/nov/04/uk-million-selling-singles-full-list#data for song list
* https://en.wikipedia.org/wiki/AFI%27s_100_Years...100_Movies for film list
* https://www.randomlists.com/ for random list of words
* https://en.wikipedia.org/wiki/List_of_best-selling_books for list of books
* https://www.scaler.com/topics/how-to-clear-screen-in-python/ for info on how to Clear User Screen depending 
  on operating System 
* https://emojicombos.com/fire-ascii-art AND https://asciiflow.com/ ASCII Art