# coursera-downloader (working - updated 01/12/2018)

Coursera Downloader - A simple automation script to download, label and arrange Coursera videos in ascending order.



## Features
- [x] Download tutorial videos in mp4 format
- [x] Name the videos according to the video title
- [x] Arrange the videos in ascending order with numbering
- [ ] Download subtitles (will be added soon)



## Getting Started
### Prerequisites
- Python 3 and above
- Enrolled in the course and have the course you want to download in the coursera website **Last Active** list


### Installing

- Install selenium
```
pip install selenium
```

- Install requests
```
pip install requests
```

- Install Mozilla Firefox browser

- Download [geckodriver v0.23.0](https://github.com/mozilla/geckodriver/releases/tag/v0.23.0)
  1. Extract **geckodriver.exe** from the zip file
  2. Cut and paste **geckodriver.exe** into a folder that already exist in environment PATH
  
  Windows example using terminal:
  ```
  move C:\Users\bcbcbcbcbcl\Desktop\geckodriver.exe C:\Users\bcbcbcbcbcl\AppData\Local\Programs\Python\Python37-32\
  ```
  
  Linux example using terminal:
  ```
  sudo mv geckodriver /usr/local/bin
  ```

- Download [**coursera-download.py**](coursera-download.py) from this repository and place it in the directory you want to store the courses



## Start downloading

Open up terminal and type
```
python /path/to/the/script/coursera-download.py -u {username/email} -p {password}
```

Windows example:
```
python C:\Users\bcbcbcbcbcl\Desktop\coursera-download.py -u youremail@gmail.com -p yourpassword
```

Linux example:
```
python /home/bcbcbcbcbcl/Desktop/coursera-download.py -u youremail@gmail.com -p yourpassword
```


And enter the coursename you want to download exactly as shown in website. For example, to download "Sequence Models".
```
Please enter the coursename you want to download exactly as shown in the website: sequence models
```
(Make sure it is in your courses **Last Active** list and you have enrolled the course)

Please be noted that this script is only use to download all videos in one course per time but not all courses in one specialization.


### Other options
You may set the waiting time for web elements longer if your internet connection is very slow and take longer time to load a website. You can also set it faster if you have very fast internet connection. Recommended minimum waiting time is 5 seconds even you are having very fast internet connection to allow the web page some time to load. 

Turn off headless mode will open up mozilla browser and allow you to see the automation script crawl videos from the website.

```
-t Time for selenium web driver to wait for missing element(s) implicitly   (default: 10)
--headless-mode-off Headless mode (download the tutorial at background without open up the browser)

Example:
python coursera-download.py -u youremail@gmail.com -p yourpassword -t 20 --headless-mode-off
```

Feel free to reach out for help if you face any difficulties while downloading the courses.

Do notify me if there is any changes on the Coursera website structure caused the script not working. Thanks :heart:



## Authors

**bcbcbcbcbcl** - *Initial work* - [coursera-download](https://github.com/bcbcbcbcbcl)



## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
