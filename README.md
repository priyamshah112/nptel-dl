# nptel-dl
A small command-line program to download lecture videos from nptel.ac.in 

==================================================================
##Installation

####From Source
* Clone the repo or download the zip
* Make sure you have pip installed
* `cd` to the folder
* `pip -install -r "requirements.txt"`

##Usage 
* nptel-dl.py [-h] [--url URL] [--dir DIR] [--mp4] [--3gp] [--limit] [--include] [--exclude]
* The default directory is the current working directory and the default format is flv.
* On the terminal or Command Prompt Type
   'python nptel-dl.py --url "url" --dir "directory" --mp4'
* The --include option overrides the --exclude option.
* Example : python nptel-dl.py --url 'http://nptel.ac.in/courses/108103007/' --dir 'D:\Tutorials' --mp4

#Options
      -h, --help  show this help message and exit
      --url URL   The URL to download videos from.
      --dir DIR   The directory to save videos in. Default value is the current working directory.
      --mp4       Download in MP4 format.
      --3gp       Download in 3GP format.
      --exclude   exclude a specific list of videos.(list of space separated inteers)
      --include   Download a specific list of videos.(list of space separated integers)
      --limit     limit the number of videos.(Single integer)
      --range     Range of videos to download.(Two space separated integers.)
  
###Dependencies
* BeautifulSoup - For HTML parsing
* Requests - for retrieving HTML
