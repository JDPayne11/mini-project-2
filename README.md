# Miniproject 2

### [Assignment](assignment.md)

## Project/Goals
My goals for this assignment are to compare 2 different APIs based on their ability to find POI data in Nashville Tennesse.

## Process
### (your step 1)
I used documentation on yelp and foursquare to find points of interest in a 1km radius 
I then parsed through both responses to find import information such as name, location, category, reviews, and rating
I then created a table for foursquare and another for yelp
Finally I merged both dataframes into a SQL database and a single pandas Dataframe
### (your step 2)
My metrics:
    Which API retrieved more responses?
    Which API recieved more information on individual POIs?
    What were the differences in venues stored by each API?

## Results
(fill in what you found about the comparative quality of API coverage in your chosen area)
Both API's had a limit of 50 responses
Yelp recieved information on reviews and ratings while Foursquare did not
13 places were found in both APIs



## Challenges 
(discuss challenges you faced in the project)

I tried using the get place details API after getting fsq_id information from the places search API. I thought the place details API would give me more information such as the rating. However, it returned the same information.

Moving data from the pandas dataframe to SQLite was difficult as they're both languages/libraries im new to. I think I was making silly syntax errors which took some time to figure out.



## Future Goals
(what would you do if you had more time?)

I would further flesh out what categories means. Many categories could have been grouped under restaurant or museum but weren't
which made it harder to make conclusions on the types of venues pulled from each API

I would have cleaned up my code and put it into 1 single function that had the inputs lat,long,radius, and limit which would allow scalability