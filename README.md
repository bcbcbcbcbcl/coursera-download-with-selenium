# Coursera-download (working - updated 14/9/2018)

A simple automation script to download, label and arrange Coursera videos in ascending order.


## Features
- [x] Download tutorial videos in mp4 format
- [x] Name the videos according to the video title
- [x] Arrange the videos in ascending order with numbering
- [ ] Download subtitles (will be added soon)


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

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

- Download [geckodriver v0.20.1](https://github.com/mozilla/geckodriver/releases/tag/v0.20.1)
  1. Extract **_geckodriver.exe_** from the zip file
  2. Cut and paste **_geckodriver.exe_** into selenium folder

- Download [**coursera-download.py**](coursera-download.py) from this repository and place it in the directory you want to store the video


## Start downloading

Run the script to start download

- Open up terminal and type **python /path/to/the/script/coursera-download.py -u <username/email> -p <password/>**

Windows example:
```
python C:\Users\bcbcbcbcbcl\Desktop\coursera-download.py -u youremail@gmail.com -p yourpassword
```

Linux example:
```
python /home/bcbcbcbcbcl/Desktop/coursera-download.py -u youremail@gmail.com -p yourpassword
```

- Enter the coursename you want to download exactly as shown in website (Please make sure it is in your courses **Last Active** list)
```
Please enter the coursename you want to download exactly as shown in the website: **sequence models**
```

Feel free to report any bug in the automation script or reach out for help if you face any difficulties while downloading the courses.


## Message
I believe education should be affordable for everyone. Download the courses and learn offline to save more.
Please share it with your friends if you found this useful. Thanks :heart:


## Authors

**bcbcbcbcbcl** - *Initial work* - [Coursera-download](https://github.com/bcbcbcbcbcl)


## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
