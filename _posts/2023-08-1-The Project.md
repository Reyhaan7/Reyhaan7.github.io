I decided for my project to be in web scraping and text analysis as this is more likely to be useful for me and my field of study in the future. As I'll be doing another project soon that involves dealing with Shahname (the greatest epic in Persian literature), I decided to start with scraping this text. My project (for another course) is conducting research on the word "پند" (which can be translate to “advice”). I wasn’t sure if I must first search for this word on the website, then start the scraping or scrape the whole text (the whole book) and then continue the rest of the process. If I remember correctly from the class, we first searched for the word “sport” in the muslimahmediawatch.org then did the rest of the work. Anyways, if I wanted to scrape the whole website I had to deal with a huge data most of which I don’t even need. So I searched for my word so I had only a few pages to scrape. 
I decided to not start with OpenRefine because I have always had problems with it even in the class. I don’t know if I didn’t learn how to work with it properly at the end, or it’s really not that user-friendly and easy to use. So I started with python because I have already had some experiences and I have also worked with the library beautifulsoup. I watched a few YouTube tutorials and started importing libraries and writing codes in python. I first used the website[
](https://ganjoor.net/ferdousi/shahname) which is verey strong in collecting Persian poems. I think I was struggling with scraping data from this website for a  week or so, finally me and chatgpt gathered that the problem is the website! I think maybe I needed to know a bit more advanced programing, and codes I asked from chatgpt didn’t work either. Anyways, as I found working with this website tricky so I thought maybe I should try a different url. I[ ](http://rira.ir/) 
used[ ](http://rira.ir/) this time and searched for my selected word in the part for Shahname. This also took me more time than I predicted but finally I could save the text of the website in a txt file as well as a csv file. Then I tried to do some analysis using the nltk library. I wanted to know how many time the word پند appears with it’s synonym اندرز. I checked[  ](https://guides.library.duke.edu/c.php?g=289707&p=1930854) to get some idea on text analysis. I thought sentiment analysis looks interesting so I asked chatgpt because I had no idea how to write the appropriate code for this. After some trial and errors and installing and trying different libraries and functions, turned out all parts of my data have neutral sentiment score, it might be because the word itself is probably neutral on its own and not much negative or positive. Then I used something called average_perception_tagger in the nltk library to study how frequently the word پند   is applied along with a verb in first person singular form.
![python code](https://github.com/Reyhaan7/Reyhaan7.github.io/blob/main/assets/image/Untitled9.png?raw=true)


![python code2](https://github.com/Reyhaan7/Reyhaan7.github.io/blob/main/assets/image/Untitled10.png?raw=true)


![python code3](https://github.com/Reyhaan7/Reyhaan7.github.io/blob/main/assets/image/Untitled11.png?raw=true)

![python code4](https://github.com/Reyhaan7/Reyhaan7.github.io/blob/main/assets/image/Untitled12.png?raw=true)




I then used Voyant tool to see the word frequency and build a word cloud (which I unfortunately couldn’t do in python), and I also used AntCode for sentiment analysis. It was fascinating how with two clicks and writing one word پند   it highlighted the related words in the context. For example, word اندرز   and verbs constructed from the stem داد   were highlighted which shows that the computer could understand which word is the synonym of the word I typed in the bar, and that which verbs are usually related to it even if they are in various forms. And with getting help from the regular expression option in AntCode I searched for the terms after the word پند     which contain the letter ت   so I could observe how the second person singular is addressed in the advising.

![Voyant](https://github.com/Reyhaan7/Reyhaan7.github.io/blob/main/assets/image/Untitled6.png?raw=true)

![Voyant 2](https://github.com/Reyhaan7/Reyhaan7.github.io/blob/main/assets/image/Untitled7.png?raw=true)

![Voyant 3](https://github.com/Reyhaan7/Reyhaan7.github.io/blob/main/assets/image/Untitled8.png?raw=true)

![AntCode](https://github.com/Reyhaan7/Reyhaan7.github.io/blob/main/assets/image/Untitled1.png?raw=true)

![AntCode 2](https://github.com/Reyhaan7/Reyhaan7.github.io/blob/main/assets/image/Untitled4.png?raw=true)




And I tried jsLDA tool for topic correlation, the result was really interesting for myself.

![jsLDA](https://github.com/Reyhaan7/Reyhaan7.github.io/blob/main/assets/image/Untitled5.png?raw=true)
