# OTT Apps (Source Code Coming Soon to this public Github Repo)

### IOS and Android OTT App (Chat, Voice, Video) supports one on one and one to many.

### Goal

The approuch here is to open source the Apps and Web services sifde of things and integrate with as many different CPaaS providers as possible (e.g. Twilio, Sinch, Restcomm, Etc..) we think there is no value today of building another SIP/WebRTC backend, we want to give a head start to developers that need a working IOS, Android app for group and one to one messaging, conferencing, and voice calling.


Live Demo on App Store: https://itunes.apple.com/us/app/o2-app/id1363104848?mt=8

Tested on over 32k Live Users: https://ottusers.telecomsxchange.com 


![alt text](https://ott.telecomsxchange.com/appflow1.jpg "App Flow")



XCode view: 
![alt text](https://user-images.githubusercontent.com/26701933/79405928-5c667400-7f9e-11ea-8a46-7ec0dbdb37bc.png "X Code Ciew")


Signup:

- Ready to use your Twilio Account SID - Token for sending OTPs
- Can easily switch signup OTPs to your own HTTP API.

Video Calls:

- Twilio Programmable Video Dependant (Up to 4 people at the same time currently supported)
- Possible to use another SDK for initiating videos

Audio Calls 

- Up to 10 participents at the same time
- Twilio support already built in for Audio, Possible to switch to another SDK


Chat 

- Unlimited particpents support
- Audio Voice Message support
- Image Sharing support
- Location Sharing Support





======================== **Third Party libraries implemented** ============================

1. TwilioChatClient --> TwilioChatClient is use to for chat
2. TwilioAccessManager --> TwilioChatClient is use to hand twili token even like expire, update etc
3. TwilioVideo --> O2 use TwilioVideo for video & audio call, video & audio conference
4. GooglePlaces
5. GooglePlacePicker
6. GoogleMaps --> Google Map & Place API use to send curren or other location on chat
7. Fabric
8. Crashlytics --> Fabric use for crash report of O2 app.
9. Alamofire --> Alamofire user for webservice call
10. SwiftyGif --> SwiftyGif use to show gif image
11. SKPhotoBrowser --> SKPhotoBrowser use for create O2 folder on Photos app of device
12. SwipeCellKit --> SwipeCellKit use on table view for swipe on tableview cell
13. DropDown --> DropDown show dropdwon on Chatlist screen for short cut of video & audio conference
14. SlackTextViewController
15. SwiftRangeSlider'


### Web Service URL

=============== Chat Client====================
- Token URL For ChatClient : "https://[DOMAIN]/backend/ws/index.php/token"

=============== Group video & Audio call and Conference  ====================

identity = user mobile no with contry code
roomName = roomname is any unique roomname

Token URL For video = "https://[DOMAIN]/backend/ws/videoToken?identity=%@&roomName=%@"

=============== End ===================================================


### IOS environment setup

```shell
git clone project
```

```shell
cd project-directory
```

```shell
brew install cocopods
```

```shell
pod install
```

Open workspace file in Xcode 10.1 (Later version do not support Swift3)

### Android environment setup

TODO

