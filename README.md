# Campus Monitoring System
To start with Firebase, a google account is needed. With this Google account, Firebase
account is linked and a home page appears. There are steps which are needed to be carried
out to successfully to connect the node MCUs to the firebase and then subsequently to the
web page.

### Step 1: 
Create a new Project on Firebase named Utility Information System



### Step 2: 
Copy the host name or the project name to the arduino sketch file.
#define FIREBASE_HOST "utility-infromation-system.firebaseio.com"




### Step 3: 
Adding database secret key to the arduino sketch.
Go to Setting then Project Setting>>SERVICE ACCOUNTS>>DATABASE Secretes.
Copy "Database Secrets" as Shown in above image.
Copy and paste Database Secrets at the line in code
#define FIREBASE_AUTH
"examplesd2asdasdasdasd2asd3asdsdfsfsfvsdv32das3d2as2da3"


### Step 4: 
Add Router name and password

#define WIFI_SSID "Wifi Router Name"
#define WIFI_PASSWORD "Router Password"


## Connecting HTML page and firebase

A connection needs to be established between the two for successful data communication.

### Step 1: 
Create a project on the firebase console which in this case is Utility information system.

### Step 2: 
Create an HTML file with all the aesthetics and the variable fields that are need to be
displayed. This HTML design can be created in multiple ways either by using templates or
going from scratch.

### Step 3: 
The firebase project needs to be configured and initialized. There are option to add
firebase to android app, iOS app and webpage as well. After choosing the webpage connection,
a set of code lines are available which needs to be added to the HTML file.


### Step 4: 

The variable reference needs a set of code lines

var p1=document.getElementById('p1');
var dbRef=firebase.database().ref().child('distance');
dbRef.on('value',snap=>p1.innerText = snap.val());

### Step 5: 
The variable in this case is p1 which is added in the HTML file. The variable ‘distance’
is what we see in the firebase real-time database.
