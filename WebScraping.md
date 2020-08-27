## Comments to LC lesson in Webscraping
Are ethical considerations included/introduced in the lesson?
What is one-based indexing - terminology fylder meget i denne module evt. opdatere lektion, java consol i Chrome ser meget anerledes ud end i eksemplet i lektionen
The example with Scrapy is outdated, look evt. as this tutorial instead from March 2020: https://www.scrapehero.com/how-to-scrape-data-using-scraper-chrome-extension/

## webscraping with scrapy and Git
The following tutorial is adapted from: https://docs.scrapy.org/en/latest/topics/developer-tools.html
# Getting started
Install the Scrapy extension
Open webpage https://quotes.toscrape.com
Right click on a quote and click "undersøg/inspect"
In the Xpath the area you are interested in is highlighted. Use the arrows by the tags to expand the tags and see the hierarchy

In Git write the following:
$ scrapy shell "https://quotes.toscrape.com/"

# Scraping a single piece of information/text
Back on the webpage and in the Xpath right find the highlighted xml that corresponds to your chosen text
right click on the SPAN tag, select Copy XPath

In Git write the following:
response.xpath('insert copied xpath here/text()').getall()
The result should be something like this:
>>> response.xpath('/html/body/div/div[2]/div[1]/div[1]/span[1]/text()').getall()
['“The world as we have created it is a process of our thinking. It cannot be changed without changing our thinking.”']

Adding text() at the end we are able to extract the first quote with this basic selector. But this XPath is not really that clever. All it does is go down a desired path in the source code starting from html. So let’s see if we can refine our XPath a bit

# A more clever approach
On the webpage, in Scrapy you can see the pattern of the XML. I has identical div tags that use the same attributes and structure. There are two SPAN tags and one DIV tag.
You can expand each SPAN tag with the CLASS="text" inside the DIV tags to see each quote. Using this knowledge we can refine the XPath and select all the SPAN tags
which have the CLASS="text" attribute and scrape all our quotes at once. For this you use the has-class extension

Write the following code in Git:
 response.xpath('//span[has-class("text")]/text()').getall()
 
You should get a result like this:
>>> response.xpath('//span[has-class("text")]/text()').getall()
['“The world as we have created it is a process of our thinking. It cannot be changed without changing our thinking.”',
'“It is our choices, Harry, that show what we truly are, far more than our abilities.”',
'“There are only two ways to live your life. One is as though nothing is a miracle. The other is as though everything is a miracle.”',
...]

# Searching for information (text, words, etc) in the Scrapy Xpath
Use Ctrl+F and the search terms are highlighted in the Xml

# Setting up the pagination extension
Her hopper kæden af for mig. Dette arbejder jeg på

# Saving the scraped quotes as a file for further analysis
How to save the scraped information as a file in GIT??

