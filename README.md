# Packages
Packages you need to install to run this code are listed below: <br />
### Pip <br />
* Here is the [link](https://pip.pypa.io/en/stable/installation/) to check how to install pip
### Python <br />
* [Python for Ubuntu](https://docs.python-guide.org/starting/install3/linux/)
* [Python for Mac](https://www.python.org/downloads/macos/)
* [Python for Windows](https://www.python.org/downloads/) 
### Pandas <br />
* Here is the [link](https://pandas.pydata.org/docs/getting_started/install.html) to check how to install pandas.
### Regex <br />
* Here is the [link](https://learnbyexample.github.io/py_regular_expressions/regex-module.html) to check how to install regex.

# Description
This is a program to find the degree of profanity for given tweets. <br />
* A file with tweets in csv format is imported
* The tweets are then cleaned to remove noise from the tweets 
  * To clean the tweets hashtags, mentions, puntuations, and numbers are removed 
* A custom list of racial slur words is created
  * Words can be added, removed or imported as per requirement
* Each tweet in the imported file is then checked for racial slur words in the list
* If racial slur words are found, then based on number of racial slur words contained in the tweet, a profanity score is assigned to the tweet

# Assumptions
The following assumptions are made for this code. <br />
* The racial slur words in tweets occur with standard english spellings (NOT in forms like f*ck, b!tch etc.)
* The list of profane words are also in standard english
* The degree of profanity is assumed to be relative to the length of the tweet
* No NLP/ML methods are used in the calculation of the degree of profanity    

# Example
```
Enter a sample tweet: !!RT @dude stop writing fake %^%%78*  news asshole!!!*** 
Cleaned sample tweet:        stop writing fake        news asshole  
Sample tweet tokens:  ['stop', 'writing', 'fake', 'news', 'asshole']
Profanity score for given sample tweet is: 0.2
```



