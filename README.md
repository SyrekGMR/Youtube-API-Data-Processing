# Youtube-API-Data-Processing

<p align="center">
  <img src="Assets/YT_Logo.png" width="200" height="200" /></img>
  <img src="Assets/MongoDB_Logo.png" width="300" height="200" /></img>
</p>

This project looks to produce a reliable view-count prediction tool for Youtube videos. The aim is to monitor the number of views throughout the hours following a video upload in an attempt to produce an effective forecast into the future, allowing for the prediction of the view count at a given time. Any such prediction will be subject to factors which would prove difficult to effectively model, hence it will only focus on trends in the number of views, likes/dislikes and comments.
<br><br>
There appears to be no publicly available view-count data based on time, this required the view count to be obtained directly from Youtube at each time-step. This was done using the YoutubeAPI which facilitates HTTP requests, allowing for various queries. As this data collection task would be required to run continuously for extended periods of time, it was decided to perform this on a VM. Consequently, this data had to be stored somewhere, due to the "online" nature of the data collection task this was done using a MongoDB cluster, allowing for a connection to be established between the VM and database in only a few lines of code. Furthermore, the no-SQL database allows for more intuitive storage of the data using the JSON format.

Project Roadmap
- [x] Cluster Code Setup
- [x] Youtube API
- [ ] Data Collection / Processing
- [ ] Model Selection
- [ ] Results Evaluation
