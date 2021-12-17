ZeroSMS
=======

ZeroSMS is a proof-of-concept demonstrating a way to send Class 0 SMS on android >=2.3.

/!\ This application only works on rooted phones.

How to install
--------------

Simply use adb to drop it onto your phone:

    adb remount
    adb push ZeroSms-signed.apk /system/app

And voila !

How to use it
-------------

Type in a phone number (no phonebook pickup, this is a PoC) and a text, then press "Send SMS !". Your SMS is sent.


Greetz
------

Vorex & Kaiyou



占坑
-----
1.android 10有没有可能成功发送class 0 短信？  
2.diy Rom ？  
3.其他通用手段  



相关资料
----
1. [stackoverflow - Class 0 SMS (flash SMS) on Android ](https://stackoverflow.com/questions/9123125/class-0-sms-flash-sms-on-android/)