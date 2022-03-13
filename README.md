# Dorksqueezidy
Just a webpage and python script to control Squeezelite players, play Internet Radio stations and monitor your pi using RPIMonitor as an addon.  you'll need to alter the html to point to your LMS server for Squeezelite players, and the local raspberry pi hostname.  You'll have to install RPI Monitor separately.

![dorksqueezidy](https://user-images.githubusercontent.com/16979775/158045440-a7e93a65-2f28-4f58-9eb9-45340cdd684f.png)

Instructions : Download python file, index.html, and moodies.csv files. Create a folder on the server pi, ie. "dorksqueezidy", with a subdirectory for templates, (a flask thing) where the index.html bootstrap file should reside. The csv file will reside in the same folder as the python file. Note there is a reference or two in the python file to the html page, so rename at your risk, but not a big deal.

Must have Prerequisites include  MPD, MPC, Pip3, python3, Flask, and Tornado.  Optionals are RPI Monitor and Squeezelite. If you're a Squeezelite and Logitech Media Server fan as I am, you'll need a running pi acting as a LMS Server.  This will enable multiple squeezelite players for a whole house audio.  Just note the IP address of your LMS server and replace the index ip address in the html file with your servers address. See screenshot.  
Once you have all the programs loaded and the files in place, simply run the python program from the command line. A one line indicator on the command line will alert you when it is OK to navigate to the web page. Navigate to the serving Pi's ip address at port 8080( for example "10.0.0.112:8080") using a web browser. Hit a play button and that should be it. Check your mpd.conf or soundcard settings if no audio eminates from your speakers.
![config2](https://user-images.githubusercontent.com/16979775/158045286-654498fb-1003-40e3-a69c-bc19be38262f.png)
