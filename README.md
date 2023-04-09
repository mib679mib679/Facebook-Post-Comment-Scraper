# Facebook-Post-Comment-Scraper
A Facebook Post and comment scraper without using API.

#### Keyword: Web Crawler, Data Engineering, Selenium, BeautifulSoup, Web Automation, HTML and CSS syntax.  

#### File description:
Bardeen教學.pdf - An instruction of using Bardeen to extract ID, in Chinese.    
Python腳本操作教學.pdf - An instruction of how to use Python script to extract the contents, in Chinese.      
scraper_for_multipleID.ipynb - This file contains the code that can extract all the post contents and comments for a list of IDs.     
scraper_for_oneID.ipynb - This file contains the code that can extract all the post contents and comments for single ID.      
保養品ID.xlsx - An excel file that was scraped by Bardeen for test purpose.      
第一批Post_content.csv - A csv file that contains the test result of this scraper.       

This is a Facebook post and comment scraper I made for a friend who runs an e-commerce company called Morning Shop in Taiwan, They wanted to gather posts and comments from various internet celebrities's fan pages to determine which influencers would be valuable for endorsements.
The project has two versions: one for single ID and another loop version for multiple IDs. This method does not require the use of any APIs.


The process can be divided to 4 steps below:
1. Use Chrome extension - Bardeen to scrape some Facebook search result, there is a video on Youtube for this (https://www.youtube.com/watch?v=vVSPVC1Jv38&t=117s), you need to get the name and link to fanpage for each internet celebrity to proceed. The output will be an excel file.

2. Use this Python Script to read the excel file and extract the IDs of each internet celebrity.

3. Keep running the Python Script to automatically open an additional Chrome browser and log-in to Facebook, extract the URLs for each internet celebrity's most recent post and corresponding comments, you can specify how many times to scroll down to load more posts as many as possible. This process requires you to open the additional Chrome browser until the cell finishs the operation.

4. After getting all the URLs of each post, run the final cell to extract all the post contents and comments into a csv file. This process do not require to open the additional Chrome browser, you can minimise the browser and keep doing your work. 
