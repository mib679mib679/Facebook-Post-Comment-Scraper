# Facebook-Post-Comment-Scraper
A Facebook Post and comment scraper without using API.

Keyword: Web Crawler, Data Engineering, Selenium, BeautifulSoup, HTML and CSS syntax.   

This is a Facebook post and comment scraper I made for a friend who's operating an e-commerce company, they would like to get all the post and comments from some internet celebrity's fanpage, in order to distinguish who is worth to hire for endorsement.
There are two version of the project, one is for single ID, another one is a loop version for all the IDs. This method does not need any API.

The process can be divided to these parts below:
1. Use Chrome extension - Bardeen to scrape some Facebook search result, there is a video on Youtube for this (https://www.youtube.com/watch?v=vVSPVC1Jv38&t=117s), you need to get the name and link to fanpage for each internet celebrity to proceed. The output will be an excel file.

2. Use this Python Script to read the excel file to extract the IDs of each internet celebrity.

3. Keep running the Python Script to automatically log-in to Facebook in an additional Chrome browser, extract the URL for each internet celebrity's most recent post and corresponding comments, you can specify how many times to scroll down to load more posts as many as possible. This process requires you to open the additional Chrome browser until the cell finish the operation.

4. After getting all the URLs of each post, run the final cell to extract all the post content and comment into a CSV file. This process do not require to open the additional Chrome browser, you can minimise the browser and keep doing your work. 
