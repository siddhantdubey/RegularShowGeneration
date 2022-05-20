# Regular Show Episode Generation

The files in this repository serve to generate new episodes of Regular Show by using Markov Chains constructed with data from all 8 seasons of the original show. 


## Getting Data 

The process of obtaining data was pretty simple. The fandom wiki for Regular Show contained [transcripts](https://regularshow.fandom.com/wiki/Category:Transcripts) for most episodes which meant that I just had to scrape the site. This is taken care of in `GetData.ipynb`. The idea behind the code is really basic:
- get every link on the page
- go to those links and get all paragraph elements
- if that element belongs to the script (if it contains parentheses or a colon and is not another link) add it to a list of lines
- write this list of lines along with newline characters to a txt file in the data folder.
This was also quite easy to implement and fandom's website cooperated nicely which is always great when you're web scraping. However, 21 episodes were unable to be obtained to character encoding problems that I decided weren't worth delving into. In total, there are 209 text files worth of data to construct models with.

## Preprocessing

## Tokenizer

## Markov Chain 

## To-Dos:

-  [ ] Obtain Data 
-  [ ] Preprocess Data 
-  [ ] Tokenizer 
-  [ ] Markov Chain
