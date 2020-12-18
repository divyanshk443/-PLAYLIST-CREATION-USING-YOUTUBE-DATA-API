## PLAYLIST-CREATION-USING-YOUTUBE-DATA-API


### API used :
1. Youtube.search.list
2. Youtube.videos.list

Firstly I had use the youtube.search.list api to get the video id and video title of my respected
query. And then using the video id in youtube.videos.list api I got all the statistics part of my
video and also the duration part.

### Filter used :
1. youtube.search().list( q=query,part='id,snippet',maxResults=50,
pageToken=next_page_token)
2. youtube.videos().list(id = video_id,part = "id, snippet, contentDetails, statistics")

### Challenges Faced:
1. In converting the statistics part into a list of dictionary .
2. Again and again exhaustement of Daily searching quota query of api.
3. In Data analysis and manipulation part: because there was some colons present
around integers and also some unwanted string in viewcount, likecount etc
( Brief Mentioned in the Notebook under the markdowns )


### From this data analysis exercise I learned:
1. How to collect the data from Youtube Api and how with the help of this youtube api
we can get the list of top videos of my query then what we do with the normal
youtube search browser.
2. How to practically manipulate the data and then do the visualization and analysis part
in it.
