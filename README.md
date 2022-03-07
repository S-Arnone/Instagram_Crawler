# Instagram Crawler
## Created By Samuel Arnone-Roller

By utilizing the crawler uploaded to this repository, you will be able to collect data on Instagram posts which is made available when browsing tags or the posts made by a specific user. This data includes: The post URL, the poster's username, the date the post was created on, a description of the post image, and the time collected (displayed in CSV as hashes, but contains workable data).

![image](https://user-images.githubusercontent.com/97333090/157091815-6ba05471-d312-40fd-ab8d-dde0de186283.png)

Due to the complexity of avoiding crawler detection, this program works through analyzing HTML which you download manually. Depending on your perspective, this can be an advantage or a disadvantage: as while slightly more work is required of you, it is possible to refine your results by selecting exactly where you wish your data to stop. In order to download this HTML, your first step should be to right click on your desired page and select 'Save as', 'Webpage, Complete'. This will download both the HTML which the crawler will be making use of, and the images associated with posts - which, while inaccessable to the bot, can be used in other complementary ways.

![image](https://user-images.githubusercontent.com/97333090/157092529-e8cb0f64-c2a1-4e8c-bc91-ee20308cb916.png)

From here, you need to get the HTML associated with this download to the crawler by one of two means:
First, you can manually upload the HTML to Google Colab, by navigating to 'Files' and 'Upload Files' (Highlighted) and uploading the HTML which you have just downloaded.
Note, however, that this will require you to comment out the 'bot.get(url)' line.

![image](https://user-images.githubusercontent.com/97333090/157093186-4de77938-63f8-492d-88ea-4ae05f1258ab.png)

Second, you can upload your HTML to google drive, and copy the download link which comes up when you select 'download'. This can be somewhat tricky due to timing, but is possible. If you experience significant difficulty, it may be helpful to record your screen as the download page is displayed and type this url in yourself. Though it may seem possible to do so, you cannot use the link referencing the location of the HTML in your google drive - as the HTML and JavaScript of the surrounging page will be enmeshed with the HTML saved from Instagram - corrupting it.

![image](https://user-images.githubusercontent.com/97333090/157093691-97fc9a0d-2a17-4209-996f-3aef55b4f002.png)

Finally, enter the name of your file by replacing 'CrawlerDataWIP' with your desired name.

![image](https://user-images.githubusercontent.com/97333090/157104641-8af4229c-8c58-4aad-b955-95da3694ef74.png)

From here on, nothing is required of you; the crawler will be able to process the HTML and produce a neat CSV containing your results. Be warned, however, that depending on the language which you are crawling, you may need to transform your CSV by selecting 'Data', 'From Text/CSV', your csv file, 'Unicode UTF-8' and 'Load'. 

![image](https://user-images.githubusercontent.com/97333090/157094192-73b7913c-d112-471e-82b7-b856860ffda0.png)

In the end your work will be rewarded with a CSV!

![image](https://user-images.githubusercontent.com/97333090/157105064-4ca20f80-3c58-4d19-b7c0-31f8d0f1ed38.png)

