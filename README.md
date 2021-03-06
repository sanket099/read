# Covid App
### Resources Used 

##### We are using the free versions of the following resources in our prototype, However if one wants to scale up, the descriptions and pricing models are given below.

**1. MongoDb Atlas**
MongoDB Atlas is the global cloud database service for modern applications.
We have used Mongo Db to manage databases and tables in our project.
It is Flexible and scalable document database. Available as a fully managed service.

Link :   https://www.mongodb.com/cloud/atlas
Pricing :  https://www.mongodb.com/cloud/atlas/pricing
  

**2. Cloudinary**
Cloudinary is an end-to-end image- and video-management solution for websites and mobile apps, covering everything from image and video uploads, storage, manipulations, optimizations to delivery.
The company provides a cloud-based image and video management services. It enables users to upload, store, manage, manipulate and deliver images and video for websites and apps. 

We have used cloudinary to upload and get images of products in our project.
 
Link : https://cloudinary.com/
Pricing :  https://cloudinary.com/pricing


**3. Pusher**
Pusher makes communication and collaboration APIs that power apps all over the world supported by easy to integrate SDKs for web, mobile, and backend.
We are using pusher to send and recieve notifications in our project.

Links : https://github.com/pusher
https://pusher.com/

Pricing : https://pusher.com/channels/pricing

**4. MailGun**
Powerful APIs that enable you to send, receive and track email effortlessly.
We have used mailgun to send secure emails. 
Link : https://www.mailgun.com/
Pricing : https://www.mailgun.com/pricing/

**5. Heroku**
Hosting Service 
Heroku is a platform as a service (PaaS) that enables developers to build, run, and operate applications entirely in the cloud.
We are using heroku to host our api on the cloud.

Links : https://www.heroku.com/
Pricing : https://www.heroku.com/pricing

* One alternative to Heroku for hosting is DigitalOcean :  https://www.digitalocean.com/ 


**6. Nexmo**
We are already using MailGun for sending secure emails to register a new user and in the forgot password 
However if an sms service to send auth otp is required, Nexmo is suggested.
Nexmo is a service used to send and receive sms.
https://developer.nexmo.com/

##### Open-Source Resources used in the app :

1. The feature to show the current covid cases is implemented using the covid19api :
https://covid19api.com/
https://documenter.getpostman.com/view/10808728/SzS8rjbc?version=latest

2. The chips used in managing Tags of products in the project are implemented using :
https://github.com/DoodleScheduling/android-material-chips

#### We have also used Google maps SDK and Places Api
The keys for the same can be generated by visiting :
https://console.cloud.google.com/

#### Implementation of keys in the app 

Once the resources keys have been received , The pusher, cloudinary, places api keys need to be setup with android studio : 
This code snippet can be found in android_app/Project/app/src/main/res/values/secret.xml. You may add respective keys at the mentioned places : 

```
<?xml version="1.0" encoding="utf-8"?>
<resources>
    
    <string name="cloudinary" >cloudinary://api_key:api_secret@CloudName</string>
    <string name="pusher_key">"PusherKey"</string>
    <string name="pusher_cluster">"PusherCluster"</string>
    <string name="channel_name">"PusherChannelName"</string>
    <string name="event_name">"PusherEventName"</string>
    <string name="event_name_2">"PusherEventName2"</string>
    <string name="places_api">"PlacesApiKey"</string>
</resources>

```


## Android Release 


for releasing the application, visit https://play.google.com/apps/publish
Sign in with the google account 
Pay the fees to publish on play store

Here is a video which will guide through the process of publishing 
https://www.youtube.com/watch?v=AWawL5HFn64

Here is a checklist provided by Google. It brings together the processes you should follow to ensure your app is launched successfully.
https://developer.android.com/distribute/best-practices/launch/launch-checklist. 

You can find more details about the release at https://developer.android.com/studio/publish#publishing-release.










