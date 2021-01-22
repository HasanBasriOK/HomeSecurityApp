# HomeSecurityApp
Home Security Application (Arduino,Xamarin Android,Web Api)
This application has been developed to provide home security.The operating logic of the application is briefly as follows:

A camera connected to Arduino is placed in the desired area of the house and takes the image from there and sends this image to the computer it is connected to via serial port.

The application(Winform app) that takes the image uses the emgucv libraries to compare the new image with the previously trained model.

The application that receives the image uses the emgucv libraries to compare the previously trained model with the new image. As a result of comparison, 
the system generates alarm when there is a match below a certain percentage.

These alarms are:
Mobile notification
Skype call
Sending sms to the defined numbers

Management procedures for the alarm mechanism are carried out using the web application.

Finally, there are functions of location tracking and panic button in the mobile application.

With the location tracking feature, if the user did not activate the alarm while leaving the house, the user can be warned using the mobile notification.

With the panic button feature, when the user does not feel safe while outside the home, the address information of the current location is sent as sms to the previously defined numbers.

The following technologies are used in this application:
Image processing: Emgucv
Getting images from camera: arduino-ov7670
Database: MSSQL
Mobile application: Xamarin android
Mobile-DB communication: ASP.NET Web Api

![image](https://github.com/HasanBasriOK/HomeSecurityApp/blob/master/pictures/Picture1.jpg)

![image](https://github.com/HasanBasriOK/HomeSecurityApp/blob/master/pictures/Screenshot_2018-05-23-06-48-23.png)

![image](https://github.com/HasanBasriOK/HomeSecurityApp/blob/master/pictures/Screenshot_2018-05-23-06-50-31.png)

I hope it helps for you
