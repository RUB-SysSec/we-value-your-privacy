# Measuring the GDPR’s Impact on Web Privacy

From December 2017 to December 2018, we monitored the 500 most popular websites of all member states of the European Union to track privacy related changes around the enforcement date of the General Data Protection Regulation.

![Overview of the pre/post GDPR comparison](https://raw.githubusercontent.com/RUB-SysSec/we-value-your-privacy/master/EU_overview.svg)

The results of our study are published in the paper "We Value Your Privacy ... Now Take Some Cookies: Measuring the GDPR’s Impact on Web Privacy" presented at NDSS 2019.
In this repository you can find the raw data to our study. 



# Paper

Martin Degeling,  Christine Utz, Christopher Lentzsch, Henry Hosseini, Florian Schaub, and Thorsten Holz. “We Value Your Privacy ... Now Take Some Cookies: Measuring the GDPR’s Impact on Web Privacy.” In Proc. NDSS 2019. San Diego, CA: Internet Society, 2019. https://doi.org/10.14722/ndss.2019.23378.

An updated version of the paper is available at http://arxiv.org/abs/1808.05096


# Data

The following data is made public at the moment.
Be aware that we processed the data for our analysis. If you have any questions about how to work with the data or regarding replication of our results, feel free to contact us.

## Wording

`privacy_wording.json`: This file contains a list of terms to identify links to privacy policies sorted by country.

```
{
	"country": Country Code,
	"words": [Words referring to privacy policies],
	"tlds": [Top level domains],
	"GDPR": [Array of words referring to the GDPR]
}
```

## Annotation Data

`site_annotations_2017-12_2018-12`: This file contains automatic and manual annotations for the sites we crawled.

While we crawled all sites every month, they were annotated manually only in January 2018 (post-GDPR) and in May and August 2018 (post-GDPR).
For the months in between you will probably only find `NOLINKFOUND` and `DONE` status codes.


```
{
    "crawl": Month of the Crawl,
    "host": Host URL,
    "status": NOLINKFOUND|OFFLINE|DONE|NOPOLICY,
    "tracker": [List of Tracking Domains],
    "documents": [List of URLs to privacy policies]
}
```




# Contact

Martin Degeling:
* Via email: `martin.degeling@ruhr-uni-bochum.de`
* On Twitter: @mrtn3000
