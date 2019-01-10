
   

  # Portfolio
### Course : Applied Data Sciences KB-74
### Project name : Cyber Security
### Name : Jae Kyu Lee
### Birthplace : Republic Of Korea
### Student Number : 18132782
### E-mail address : dlworb1994@naver.com
###   

### Project's Objecitive 
###  -> Collecting twitter feeds and making classifier & Sentiment analysis Specified for CyberSecurity


1. ### Introduction

My name is Kyu, I'm from Republic of Korea(South Korea) and i am 24 years old.
My majors in home university(University Of Seoul) are Big-Data Analysis & Geo-Informatics.
My dream is to become an international big-data analyst who specializes in spatial data.
So i decided to take this course - Applied data science at THUAS.
I'm working on a project - Cyber Security.
I chose this project because i have wanted to analyze SNS data with Machine-learnig for a long time.

In my project me and my project mates usually use the knowledges provided by the course. For example we use python libraries Pandas and Numpy, making own fuctions etc. Because i studied python and machine-learning hard with Datacamp and Coursera, i can do my project well.
But i also use the knowledges studied by myself like library tweepy, making twitter developer ID and how to use it and sentiment analyis etc. My project is related with twitter so i have to study a lot for using and dealing with twitter to get tweet data. Also i have to study a lot with sentiment analysis with references and video clips in youtube.


2. ### Jargon
 
Frequent & Important words which are used in Cybersecurity's Work.

 * _Anonymous_.- a decentralized international hacktivist group that is widely known for its various DDoS cyber attacks against several governments, government institutions and government agencies, corporations, and the Church of Scientology.

 * _API_.- Abbreviation for application programming interface: a way ofcommunicating with a particular computer program or internet service.
 
 * _Classifier_. - The Code which is classifying things with standards

 * _Cyberattack_.- An attempt by hackers to damage or destroy a computer network or system.
 
 * _Cybersecurity_.- The state of being protected against the criminal or unauthorized use of electronic data, or the measures taken to achieve this.
 
 * _Hacktivism_.- The activity of getting into computer systems without permission inorder to achieve political aims.
 
 * _Hacktivist_.- A person who gains unauthorized access to computer files or networks in order to further social or political ends.
 
 * _Sentiment Analysis_.- The process of computationally identifying and categorizing opinions expressed in a piece of text, especially in order to determine whether the writer's attitude towards a particular topic, product, etc. is positive, negative, or neutral.
 
 * _Social media_.- Refers to websites and computer programs that make communication possible with the use of computers or mobile phones.



3. ### Data Camp assignments
Here is the proof that i finished all the courses what i had to take during this semester for 
preparing ourselfs & project. Also it was for studying developing of the Python and Machine Learning tasks.

![Datacamp_Kyu](Datacamp_Kyu.png)

![Datacamp_Kyu2](Datacamp2_Kyu.png)

![Datacamp_Kyu3](Datacamp3_Kyu.png)
                


4. ### All Data Camp Courses
Here is the courses that i accomplished in Datacamp not only what i had to take but also what i studied additionally.
    
   * 1.- [Introduction to Python Course](StatementofAccomplishment(9).pdf)
 
     * 2.- [Intermediate Python for Data Science Course](StatementofAccomplishment.pdf)
     
     * 3.- [Introduction to Data Visualization With Python Course](StatementofAccomplishment(8).pdf)
     
     * 4.- [pandas Foundations Course](StatementofAccomplishment(6).pdf)
     
     * 5.- [Python Data Science Toolbox (Part 2)](StatementofAccomplishment(2).pdf)
     
     * 6.- [Importing data in Python (Part 1)](StatementofAccomplishment(7).pdf)
     
     * 7.- [Cleaning Data in Python Course](StatementofAccomplishment(3).pdf)
     
     * 8.- [Statistical Thinking in Python (Part 1)](StatementofAccomplishment(4).pdf)
     
     * 9.- [Supervised Learning with scikit-learn Course](StatementofAccomplishment(5).pdf)
     
     
     
 5. ### Coursera
 Here is the proof that i finished Machine-Learning courses on Coursera.
 
  ![Coursera1_Kyu](Coursera1_Kyu.png)
 
  ![Coursera2_Kyu](Coursera2_Kyu.png)
  
  
      
6. ### Presentations
    Here are presentations that i did in this semester. My group did weekly presentation with one person.
    
    
     * 1.- [My first Presentation(Week5)](cybersecurity_week5.pptx)
     
     * 2.- [My Second Presentation(Week11)](cybersecurity_week11.pptx)



7. ### Python Notebooks
In this part i made some my own programmes and codes for using our project. It was for counting words like hactivist's keywords in tweets, hashtags which they use and username they advert. 

First, this code which is kind of prototype inspires me to make codes for word counting. I just tried to make basic code first and then want to understand what should i make addtionally.

   ![inspiration](inspiration.png) 
   
Before counting words, i have to extract pure sentences from twitter data. 
In this step, i made code for extracting tweets from twitter with using userID list(hacktivists, excel format) and my twitter developer ID for accessing twitter. I access twitter with developer ID and extract user's tweets who are written in my userID list. Also i extract number of retweets and likes, date of tweet and length of tweet. They are supposed to be used later, but finally we didnt use that datas. 

   ![basicsetforcode](basicsetforcode.png)
   
   This is the basic settings for using code.
   
   ![extractexcel](extractexcel.png)  
   
   This is the code for extracting tweets from twitter with using userID list(hacktivists, excel format). I have 70 hactivist's tweeter ID. It was offered by our supervisor.
   
   ![authenticationfunction](authenticationfunction.png) 
   ![tweetmining](tweetmining.png) 
   
   In this part, i made code for mining tweets from twitter. I did it with my project mate Jorge.
   
   ![result_tweets](result_tweets.png) 
   And it is the result of tweets. There are tweets, name of user, length of sentence, ID, date of tweet, source, number of likes and retweets. I supposed to use all these things to approaching our project's goal in that time, but finally i only used tweets.
   

Next step, i have to refine extracted tweets. Because if i use word counting code with not refined tweets, the result will be full with words like 'a','the','is' kind of these words that we usually use in normal sentence(not hactivst's sentence). This result will hinder our goal to extract hacktivist's word. So i made 'removig punctuation' code for refining kind of these words. 

   ![removingpunctuation](removingpunctuation.png) 
   
   In this code, stopwords.words('english') means words like 'a','the','is' etc, stopwords.words('spanish') means words like 'a','the','is' etc with spanish. And single_words is a my own list of words not contained in stopwords but should be erased from extracted tweets. I just made it because i worried that i can miss some words except stopwords. After running counter code, i add some words to single_words if i notice unimportant words in the result of counter.
   
   
After using removing punctuation code, i can get tweet sentences consist of words which are excluded unimportant words for getting hacktivist's words. 

   ![result_removing](result_removing.png)
   
Finally i created code that creates a list of the most frequently used words with pandas series. This result is very important in my project because i use this words and numbers again until end of the project to figure out graphs, compare numbers of one word between users etc. It is no exaggeration to say that creating this code accounts for half of the project.
  
   ![counter](counter.png) 
   
Additionally i created code that creates a list of the most frequently used hashtags which they use and usernmae they advert. Because of using removing punctuation, i can't figure out numbers of hashtags and usernames. Because the punction elimates special characters like @,#,$,& etc. So i have to add new sentences from counter code and change some sentences.

   ![hashtag](hashtag.png) 
   ![username](username.png)  


   
1.-Counting keyword, hashtags and usernames ok
2.-Remove unnecessary words in tweets ok
3.-divide whole tweets data with sentences ok

4.-review and label tweets with our hand
5.-make code for sentiment analysis

 
8. ### Other works 
  
In my project, me and my project mates have to make classifiers for distinguish whether user is hactivist or not. First of this step, we have to make our own hand-written sentiment classifer with 16000 tweet sentences. Because we can't get precise hactivist words dictionary so we have to make our own hactivist words dictionary with standards for our project. We labeled all tweet sentences whether it is a hactivist's sentence or not. If it is a hactivist's sentence or contained keywords from our counter code, we labeled 1. If it is a normal sentence or not english sentence, we labeled 0.

   ![criteria_sentiment](criteria_sentiment.png) 
   
   These are the examples that we labeled.
   
   ![example_sentiment](example_sentiment.png) 
   
   Because there are words like hacker, hacking contained in sentence, we labled 1. And we labeld 0 for below sentences because those are normal sentences or non english sentences.
   
   ![sentiment](sentiment.png) 
   
   This is just few part of our sentiment classifier. I labeled 2000 tweets from 11 users.
   Finally we completed labeling all the tweets, and use this sentiment classifier to next step.
   
   

9. ### Partcodes before changing objective
     
Unfortunately our groups objective was changed in November because of some problems to get knoledges and supervisor's comment. So there are not much code that we used for this group. But there are many codes that we used before changing our objecitives so i just put this codes at the end of my portfolio for proving that i did hard work on my project.

   * 1.- [a](a.pdf)
   
   * 2.- [a](a.pdf)
     
   * 3.- [a](a.pdf)
     

10. ### References

    * 1.- Eung Yong Park. (2011). Jump to Python, Easypublishing
    
    * 2.- Wes Mckinny. (2013). Python for data analysis. O'Reilly
    
    * 3.- Raúl E. López Briega. (2017). Procesamiento de Lenguaje Natural con Python. 25/10/2018, de Blog Sitio web: https://relopezbriega.github.io/blog/2017/09/23/procesamiento-del-lenguaje-natural-con-python/ 
    
    * 4.- tthustla. (2018). Another Twitter Sentiment Analysis with Python - Part 1. 26/10/2018, de GitHub Sitio web: https://github.com/tthustla/twitter_sentiment_analysis_part1/blob/master/Capstone_part2.ipynb
    
    * 5.- Alec Go, Richa Bhayani y Lei Huang (2009). Twitter Sentiment Classification using Distant Supervision,*academia.edu.9*,1-6.
    
    * 6.- Cambridge University Press. (2018). Cambridge Dictionary. 09/11/2018, de Cambridge University Press Sitio web: https://dictionary.cambridge.org/dictionary/english/
    






                
