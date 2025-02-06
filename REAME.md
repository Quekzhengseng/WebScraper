# Contains 4 scrapers, Change the firefox profiles within each to your own path!
# Log into chatgpt, quora before hand 

Quora_Answer_Webscraper
- Input questions.csv
	- Contains (Keyword, Title, Quora_Link)
	- Keyword : Genre you are finding e.g Machine Learning
	- Title : Question about that genre
	- Quora Link : Link to that question in quora
- Output Question.JSONL 
	- Contains all the answer to that specific question qithin quora

Quora_Questions_Webscraper
- Input put the topics you want to scrape here.csv
	- Contains (Topics, Genre)
	- Topic : Topic you wanna find questions on
	- Genre : The overarching topic that the directory of the file will be saved into 
- Output genre Questions/ Topic.csv
	- Contains (Keyword, Title, Quora_Link)
	- Keyword : Topic you are searching for
	- Title : Question about that topic
	- Quora Link : Link to that question in quora

Quora_GPTAnswer_Webscraper
- Input topics/topic.csv
	- Contains (Keyword, Title, Quora_Link) 
	- Keyword : Genre you are finding e.g Machine Learning
	- Title : Question about that genre
	- Quora Link : Will not be used
- Output Machine Learning GPT Answer/ {Keyword}.jsonl
	- Contains all the answers by CHATGPT to the questions formatted in a dictionary line by line


Quora_GPTQuestion_Webscraper
- Input put the topics you want to scrape here.csv
	- Contains (Topics, Genre)
	- Topic : Topic you wanna find questions on
	- Genre : Not used
- Output Machine Learning GPT Question/ {Topic}.jsonl
	- Contains all the questions by CHATGPT in a csv file line by line
	- Can be fed back into GPT answer scraper to get all the answers

# Delete everything in the other folders, thanks.
