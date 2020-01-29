## Vigilant

This project allows police and other administrative services to dynamically set up geofences in order to send push notifications to regular citizens/users. Canada currently has an emergency alert system, but it is limited both in scope and effectiveness: it fails to reach all targeted users and is only purposed for serious incidents. This Android app was developed so police could warn residents about potentially dangerous events that have happened in their area (ex. Burglary at 16th Avenue and 5th Street. Suspect still at large in this area. Exercise extra caution).

Structure:

- Front-end setup with Android Studio using Google Maps API for live user location and NotificationManager to send push notifications to users.

- Backend server setup with Firebase; Firebase Cloud Messaging used to communicate specific notification text with front-end; Firebase Webhook used to establish connection with Radar.io

- Radar.io SDK integrated for communication between front-end app and Radar


Future Potential Expansions:
- Because there is live tracking of user data already, and the location data of police-reported incidents is transferred through our backend already, we can use Cloud Firestore to store this data, interpret it w/ data analytics/machine learning to help path users in the front end with existing Google Maps API to route them on safest routes late at night
- Potentially implement video-intelligence software so that any time users take videos that triggers the software to interpret an violent incident, a geofence is set up and police services immediately contacted
