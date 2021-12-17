ZeroSMS
=======

1.android 10有没有可能成功发送class 0 短信？  
2.diy Rom ？  
3.其他通用手段  


### 相关资料

1.[stackoverflow - Class 0 SMS (flash SMS) on Android ](https://stackoverflow.com/questions/9123125/class-0-sms-flash-sms-on-android/)

2.[android-hidden-api](https://github.com/anggrayudi/android-hidden-api)

3.[Is it possible to access com.android.internal.telephony.PhoneFactory ?](https:github.com/anggrayudi/android-hidden-api/issues/37)

---

This is an internal API, this project only provides Framework hidden API now, such as android.app.StatusBarManager and etc.

Such as those APIs below are NOT included in Framework APIs:

com.android.internal.*

com.android.server.* (in service jar)

com.android.telephony.PhoneFactory is included in telephony/jar. So it not included in this project now. You can try compile AOSP yourself and find those jars in out folder.

---
