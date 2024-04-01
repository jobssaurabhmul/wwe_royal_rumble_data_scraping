# WWE Royal Rumble Data Scraping Using Selenium
Scraping Data about the WWE Royal Rumble Events
Excerpt from https://en.wikipedia.org/wiki/Royal_Rumble_match
> The Royal Rumble match is a professional wrestling match based on the classic Battle Royal match in which a number of wrestlers (traditionally 30) aim at eliminating their competitors by tossing them over the top rope, with both feet touching the floor. The match is typically the main event of WWE's January pay-per-view and livestreaming event known as the Royal Rumble. The winner of the event is the last wrestler remaining after all others have been eliminated. 

WWE Anually releases a video titled **WWE Royal Rumble: By the Numbers**

The video details interesting statistics and facts about the annual event.
Some facts include:
+ The number of winners over the years
+ The Entrant number with the highest no. of wins
+ The Entrant who has eliminated most competitors in a match.

https://youtu.be/WV2jdXzLMpQ

This Project is an attempt to recreate the above statistics by first scraping the data from the internet.
The data has been scraped from the website: https://www.cagematch.net/
Cagematch is a popular website in the world of professional wrestling, dedicated to data about this sport.

# Procedure
1. First I needed a list of the events to scrape the data from. The first event was in 1988 and the latest one was in 2024. On the website there was no particular tag or filter from which all the events were listed in one place. Hence I used the website's search functionality to get all the required events on one page. By using custom filters in python, I was able to extract the details for the required events only.
2. 
