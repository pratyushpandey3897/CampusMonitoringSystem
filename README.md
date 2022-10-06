# Campus Monitoring System
To start with Firebase, a google account is needed. With this Google account, Firebase
account is linked and a home page appears. There are steps which are needed to be carried
out to successfully to connect the node MCUs to the firebase and then subsequently to the
web page.

### Step 1: Create a new Project on Firebase named Utility Information System



### Step 2: Copy the host name or the project name to the arduino sketch file.
#define FIREBASE_HOST "utility-infromation-system.firebaseio.com"




### Step 3: Adding database secret key to the arduino sketch.
Go to Setting then Project Setting>>SERVICE ACCOUNTS>>DATABASE Secretes.
Copy "Database Secrets" as Shown in above image.
Copy and paste Database Secrets at the line in code
#define FIREBASE_AUTH
"examplesd2asdasdasdasd2asd3asdsdfsfsfvsdv32das3d2as2da3"


### Step 4: Add Router name and password

#define WIFI_SSID "Wifi Router Name"
#define WIFI_PASSWORD "Router Password"
