# spotify_songs_data_visualisation_analys

Spotify Songs
The data this week comes from Spotify via the spotifyr package. Charlie Thompson, Josiah Parry, Donal Phipps, and Tom Wolff authored this package to make it easier to get either your own data or general metadata arounds songs from Spotify's API. Make sure to check out the spotifyr package website to see how you can collect your own data!

Kaylin Pavlik had a recent blogpost using the audio features to explore and classify songs. She used the spotifyr package to collect about 5000 songs from 6 main categories (EDM, Latin, Pop, R&B, Rap, & Rock).

h/t to Jon Harmon & Neal Grantham.

Get the data here
# Get the Data

spotify_songs <- readr::read_csv('https://raw.githubusercontent.com/rfordatascience/tidytuesday/master/data/2020/2020-01-21/spotify_songs.csv')

# Or read in with tidytuesdayR package (https://github.com/thebioengineer/tidytuesdayR)
# PLEASE NOTE TO USE 2020 DATA YOU NEED TO UPDATE tidytuesdayR from GitHub

# Either ISO-8601 date or year/week works!

# Install via devtools::install_github("thebioengineer/tidytuesdayR")

tuesdata <- tidytuesdayR::tt_load('2020-01-21') 
tuesdata <- tidytuesdayR::tt_load(2020, week = 4)


spotify_songs <- tuesdata$spotify_songs
