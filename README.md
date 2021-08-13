# Get Papers Past

A notebook-based scraper to get publications from Papers Past (that isn't accessible via [DigitalNZ](https://digitalnz.org/)). This might save someone some time!

## Details from 

From the notebook:

> This notebook was designed to scrape a specific [periodical](https://paperspast.natlib.govt.nz/periodicals) from [Papers Past](https://paperspast.natlib.govt.nz/) and to create a corpus based on the OCRd text. Obviously the [DigitalNZ API](https://digitalnz.org/developers) is a better way to capture data from PapersPast, but not everything is available through the DigitalNZ.

> I've set this notebook to scrape [Forest and Bird](https://paperspast.natlib.govt.nz/periodicals/forest-and-bird). You can change it to other periodicals or newspapers (although check you can get what you want using DigitalNZ first). Note that each periodical has background information and details of copyright and/or creative commons licenses (e.g. see the [Forest and Bird](https://paperspast.natlib.govt.nz/periodicals/forest-and-bird) page as an example). 

> This scraper is set to request pages at a very conservative rate with a 10 second sleep between requests. This can be tweaked to request pages more quickly, but be aware that you will probably be blocked quite quickly. 

## Configuration and setup

From the notebook:

> The main requirement that requires configuration is [Selenium](https://selenium.dev/). Selenium is used to automate a web browser. Requests using the `requests` library were blocked immediately when I tested (including when the User-Agent was changed from the default).  

> Documentation relevant for installing Selenium and a driver is available at the [Selenium PyPI page](https://pypi.org/project/selenium/).  

> In this case I am using the [Geckodriver](https://github.com/mozilla/geckodriver) to automate Firefox. Note: [Geckodriver binaries available here](https://github.com/mozilla/geckodriver/releases).

## Create environment

This assumes you have [Anaconda](https://www.anaconda.com/) setup.

1. `conda create --name getpaperspast python=3.7`
2. `pip install -r requirements.txt`
