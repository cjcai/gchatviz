gchat conversation visualizer
=============================

Some flaky scripts to log and visualize your chat history via gchat.

1) Enable your Gmail account to allow IMAP access. Instructions: http://email.about.com/od/accessinggmail/qt/et_gmail_imap.htm

2) Install required python packages

> pip install -r requirements.txt

3) Download freetype

OSX users:
> brew install freetype 

Linux users:
> apt-get install freetype

3) Fetch chats by running the script:

> ./getchats.sh [your google email address]

Example:
> ./getchats.sh johndoe@gmail.com 

You will be prompted to enter your gmail password. The final data will be downloaded to the file called "analyzed".

Note if your default python 2.7 interpreter is not `python`, then edit `config.sh` to change the `PYTHON` variable to point to it.


Not compatible with google hangouts
-----------------------------------
Note that google's new messaging system ("hangouts") does not log messages to IMAP (despite being accessible from the web interface). Therefore, this script is unfortunately unable to download any of your conversations post hangouts migration. It is unclear whether or not google has any desire to fix this bug. 
