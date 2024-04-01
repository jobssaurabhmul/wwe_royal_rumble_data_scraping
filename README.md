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
2. I started out by scraping the data for a single event using selenium. I mostly used to search for the required objects using html tags. Once the data was scraped for one event, I looped it to cover all the events.
3. The data that was captured was:
   + Details about the event like stadium, city, crowd capacity,etc.
   + The list of winners
   + The notes of the match, which detailed the order of eliminations of the competitors
   + The results which displayed the winner and total time duration of the match
4. Issues faced -> and Solutions:
   + One match had more than 1 winner -> had to manually correct the result on my end
   + The Royal Rumble matches for Women was started in 2018 -> the data was collected using loops and if conditions
5. The data for all the Royal Rumble Events, for the Men and the Women was captured.
![image](https://github.com/jobssaurabhmul/wwe_royal_rumble_data_scraping/assets/152073191/4e720a61-b85d-474d-9555-d63e0aeee304)


## Major Issue Faced
1. Half way through the Project I realised that with the data captured, I may not be able to get a lot of the statistics that I was looking for in the first place.
2. I later realized that Wikipedia had better collated data from which I could possibly show more of the statistics.

**Hence the analytics project was converted to a Data Scraping Project**

# Analytics
Some basic analytics and data cleaning was done in the EDA ipynb.

**Results:**
1. There have been 37 Royal Rumble Annual events starting.
2. The first one was in 1988 The latest one was in 2024
3. The Cities which hosted the Event the most were: San Antonio, Texas, USA -> 4  and  Philadelphia, Pennsylvania, USA -> 3
4. The States which have hosted the Event the most: Florida -> 7  and  Texas  ->   6
5. 36 events were hosted in the USA and 1 event in Canada
6. Arenas who have hosted the event more than once

| Arena                 | Count |
| -------------         | ------|
| Alamodome             | 3     |
| Madison Square Garden | 2     |
| Wells Fargo Center    | 2     |
| State Farm Arena      | 2     |

   
