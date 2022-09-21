# How I Once Hacked Together a Kind of Solution for Monitoring Laws, Regulations, and Standards Topics on the Web 
## Time Required
### Setup
About half a day. Your mileage will vary.

### Operation
About an hour or two once or twice a week. Again expect varying mileage.

### Maintenance
I don't know yet. I just started. I'll update this with notes in a couple of months. Check back around November, 2022.

## Tech
- [RSS](https://en.wikipedia.org/wiki/RSS)
- [Google Alerts](https://support.google.com/websearch/answer/4815696?hl=en)
- [Feedreader Online](https://feedreader.com/online/#/welcome/?action=login)

## The Challenge
My large government client wants me to monitor all the relevant industry and government bodies for emerging changes to laws, regulations, and standards that might affect interoperability, but "not spend a lot of time on it". :-D

## My Solution
I am using the RSS feeds from the sites that offered one and hacking together a set of "kind of" RSS feeds for the others using Google Alerts, then using FeedReader Online to monitor the feeds, so I can check it all in one place a couple of times a week and follow up on anything of interest.

### Overview
1. Identify the sites with the information you want to monitor and the keywords you want to monitor.
2. For the sites:
    1. Find out if the site already provides a relevant RSS feed. If so, grab that URL. 
    2. If not, see if you can do some URL hacking on a relevant search page on the site that will allow you to get the information of interest. (See examples in "Useful Details".) Save the URLs you create for later.
    3. If neither of the above are options, try to find a relevant page or pages on the site that you can watch for relevant changes. Save the page URLs for later.
    4. If none of the above are options, you are out of luck. Craft keywords to find what you hoped to find on the site and test them with your favorite search engine.
3. Create or log into your [Google Alerts](https://www.google.com/alerts) account. Create alerts for each of the URLs, except the existing site RSS feeds, and set the alerts to provide the results as an RSS feed.
4. Create or log into your [FeedReader Online](https://feedreader.com/online/#/welcome/?action=login) account

### Useful Details
#### Hacking Search Page URLs 
My example uses [Regulations.gov](https://www.regulations.gov/). It doesn't have an RSS feed to monitor for newly proposed regulations; however, it does have a great search page.

![image](https://user-images.githubusercontent.com/36210507/191566310-61b5f3cb-7b93-4c75-b4da-81414bc8799c.png)

Using the page, I found that the search terms are all included in the URL which is visible from the browser navigation bar. With a little bit of playing around I was able to come up with the following URLs for monitoring for new regulations from the government bodies of interest.

    https://www.regulations.gov/search/docket?agencyIds=NIH&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=OSHA&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=SSA&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=OPM&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=BIS&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=DOC&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=NSF&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=SAMHSA&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=NIST&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=BIA&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=RITA&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=OFCCP&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=VETS&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=LMSO&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=BLS&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=PCLOB&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=OPPM&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=OFPP&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=TA&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=CMS&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=VA&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=FDA&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=CDC&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=AHRQ&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=HHS&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    https://www.regulations.gov/search/docket?agencyIds=DOD&rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage
    
I also created this URL for monitoring any new regulations related to "interoperability".

    https://www.regulations.gov/search/docket?rulemakingStages=Proposed%20Rule%20Stage%2CPrerule%20Stage&filter=interoperability

#### Creating Google Alerts RSS Feeds From Hacked Together URLs

![image](https://user-images.githubusercontent.com/36210507/191569022-960eb855-e4c0-4919-97b7-7beb04d8a9d5.png)


#### Setting Up Feedreader to 

![image](https://user-images.githubusercontent.com/36210507/191569385-f7ada3d9-63cd-4d4e-b73f-56917775d9ab.png)

![image](https://user-images.githubusercontent.com/36210507/191569670-eca6b9b3-e7d2-4fb4-a4e5-5942dfa01773.png)


