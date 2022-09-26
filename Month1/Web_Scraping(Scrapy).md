# Web Scraping with Scrapy

Web scraping (or data scraping) is a technique used to collect content and data from the internet. This data is usually saved in a local file so that it can be manipulated and analysed as needed. If you’ve ever copied and pasted content from a website into an Excel spreadsheet, this is essentially what web scraping is, but on a very small scale.
So, using scrapy we got data of amazon in a json price with product name and their prices.
Web scraping is also known as web crawling.

## In tutorial1 
Using python package “Scrapy” and code will be scraping data from web called spider.
1.	Install the package in IDE.
2.	Using terminal write: scrapy startproject file_name

## In tutorial2
Usually websites are made of HTML and CSS.
Through python program for web scraping, it goes to the web page through the link written the python code, and then it looks at the source code and searches for the book title (E.g. Becoming) by getting all the h2 HTML tags (title tags) and extracts the text.

## In tutorial3
Robots.txt and web scraping rules
You can go to any website/robot.txt (E.g.  amazon.com/robot.txt), by this you will able to see the directory that theses websites don’t want to crawl.
We can change the rules by accessing the setting files.

## In tutorial4
It’s all about installing scrapy with pycharm.

## In tutorial5
Its all about installing scrapy and setting it with VS code.

## Tutorial6
Project Structure in Scrapy.
In the structure we have Spiders which is basically a python program that scrapes other websites and will be writing code in it.
__init__ = two files which scrapy just uses for its initialization.

### 4 other important files include:
* Settings.py 
* Pipelines.py
* Middlewares.py
* Items.py


## Let’s Scrap now!

Create a new python file in Spider file.
Write the code there:
~~~ python
import scrapy

class quotesSpider(scrapy.Spider):
    name = 'quotes'
    start_urls = [
        "https: // quotes.toscrape.com /"
    ]

    def parse (self, response):
        title = response.css("title::text").extract()
        yield {'titletext': title}
~~~
### Terminal commands
* cd quotettutorial
* scrapy crawl quotes

##  Extracting data w/ CSS Selectors
In terminal write :
* scrapy shell "https://quotes.toscrape.com/" 
then in shell
 * response.css("title")
 * response.css("title").extract()
 * response.css("title::text").extract()
 * response.css("span.text::text").extract()
 * response.css("span.text::text")[2].extract()

## Extracting data w/ XPATH
In terminal write :
* response.xpath("//title").extract()
* response.xpath("//title/text()").extract()
* response.xpath("//span[@class='text']/text()").extract()
* response.xpath("//span[@class='text']/text()")[3].extract()
* response.css("li.next a").xpath("@href").extract()
* response.css("a").xpath("@href").extract()

## Web Scraping Quotes and Authors
~~~ python
import scrapy

class quotesSpider(scrapy.Spider):
    name = 'quotes'
    start_urls = ['https://quotes.toscrape.com/']

    def parse(self, response):
        all_div_quotes = response.css('div.quote')
        for quotes in all_div_quotes:

            title = all_div_quotes.css('span.text::text').extract()
            author = all_div_quotes.css('.author::text').extract()
            tag = all_div_quotes.css('.tag::text').extract()
            yield {
                'title' : title,
                'author' : author,
                'tag' : tag,
            }
~~~

## Item containers ( Storing scraped data )
Putting all the extracted data in cointainers:
    * items.py
~~~ python
import scrapy

class QuotettutorialItem(scrapy.Item):
    # define the fields for your item here like:
    title = scrapy.Field()
    author = scrapy.Field()
    tag = scrapy.Field()
    pass
~~~

~~~ python
import scrapy
from ..items import QuotettutorialItem

class quotesSpider(scrapy.Spider):
    name = 'quotes'
    start_urls = ['https://quotes.toscrape.com/']

    def parse(self, response):
        items = QuotettutorialItem()

        all_div_quotes = response.css('div.quote')
        for quotes in all_div_quotes:

            title = all_div_quotes.css('span.text::text').extract()
            author = all_div_quotes.css('.author::text').extract()
            tag = all_div_quotes.css('.tag::text').extract()
            items['title'] = title
            items['author'] = author
            items['tag'] = tag

            yield items
~~~

##  Storing in JSON, XML and CSV

* scrapy crawl quotes -o items.json
* scrapy crawl quotes -o items.csv
* scrapy crawl quotes -o items.xml

## Pipelines in Web Scraping

















 





 




