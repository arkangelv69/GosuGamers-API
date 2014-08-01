GosuGamers-API
==============

Python unofficial API/Scraper for http://gosugamers.net

#Prerequisites:
Written in Python 3.4  
pip install -r requirements.txt or do it manually with pip.  
**BeautifulSoup 4** - https://pypi.python.org/pypi/beautifulsoup4/  
>pip install beautifulsoup4  

**Requests** - https://pypi.python.org/pypi/requests/2.3.0
>pip install requests

#Example:
See examples folder  
i.e.:  
```python
def example_all_matches():
    """Example that outputs all of the matches from dota2 page"""
    ggms = MatchScraper(game='dota2')
    ggms.find_live_matches()
    ggms.find_upcoming_matches()
    ggms.find_recent_matches()

    print('Live:')
    [print(lm) for lm in ggms.live_matches]
    print(''.center(79, '='))

    print('Upcoming:')
    [print(lm) for lm in ggms.upcoming_matches]
    print(''.center(79, '='))

    print('Recent:')
    [print(lm) for lm in ggms.recent_matches]
    print(''.center(79, '='))
```

output as in 2014-07-20 18:58 : http://pastebin.com/raw.php?i=dRGZWpRw

#Usage:

Coming soon.
