                                                */ AND & OR Operator*/
                                                
Ever sung karaoke? It's a place where you sing songs with your friends, and it's a lot of fun. We've created a table with songs, and in this challenge, you'll use queries to decide what songs to sing. For the first step, select all the song titles.

# Step 1: 
Select title
From Songs;

## Step 2
Maybe your friends only like singing either recent songs or truly epic songs. Add another SELECT that uses OR to show the titles of the songs that have an 'epic' mood or a release date after 1990. (Tip: If you're not sure how to select rows where a column equals a value, remember that you can check the documentation below.)

Select title
from songs
where mood = "epic" or released > 1990;

### Step 3
People get picky at the end of the night. Add another SELECT that uses AND to show the titles of songs that are 'epic', and released after 1990, and less than 4 minutes long.Note that the duration column is measured in seconds.

select title
from songs
where mood = "epic" and released > 1990 and duration <240;
