# google-business-scraper

~~~~~~~~~~~~~~~~~~~~~~~
git clone https://github.com/iAmMrGrim/google-business-scraper.git
~~~~~~~~~~~~~~~~~~~~~~~

~~~~~~~~~~~~~~~~~~~~~~~
cd google-business-scraper
~~~~~~~~~~~~~~~~~~~~~~~

~~~~~~~~~~~~~~~~~~~~~~~
pip install -r requirements.txt
~~~~~~~~~~~~~~~~~~~~~~~

------------------------
(note the path in the below warning is different on your pc, so make sure to make the right path)

**  WARNING: The script chromedriver-path is installed in '/home/kali/.local/bin' which is not on PATH.
  Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.  **
------------------------

~~~~~~~~~~~~~~~~~~~~~~~
sudo mkdir -p /home/kali/.local/bin
~~~~~~~~~~~~~~~~~~~~~~~

------------------------
did you make the right path?
------------------------

~~~~~~~~~~~~~~~~~~~~~~~
sudo apt update && sudo apt upgrade -y
~~~~~~~~~~~~~~~~~~~~~~~

~~~~~~~~~~~~~~~~~~~~~~~
nano src/config.py
~~~~~~~~~~~~~~~~~~~~~~~

edit this part and add as many more search terms in the same format
--------------------------------------------
    {
        "keyword": "type in search term here",
        "max_results" : 50,
    },
--------------------------------------------    

------------------------
edit the config.py file with the search terms you want, how many results you want and how many bots you want to run. (i would not try to run more than 16 and even then you need a good computer and fast internet)

you can also upload this to docker and run it that way.
------------------------

~~~~~~~~~~~~~~~~~~~~~~~
python main.py
~~~~~~~~~~~~~~~~~~~~~~~

------------------------
the results are in the folder called output.

if you want emails also then i suggest emailharvester
------------------------
