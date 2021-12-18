ZeroSMS
=======

**Status**: Developing

---

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


基本到这一步，就被限制到没啥通用性了，app需要和系统app使用相同的证书。

---

[Can a telephony.Phone object be instantiated through the sdk?](https://stackoverflow.com/questions/2143754/can-a-telephony-phone-object-be-instantiated-through-the-sdk)

[How can I sign Android application with AOSP certificate](https://stackoverflow.com/questions/57870911/how-can-i-sign-android-application-with-aosp-certificate)

[java.lang.SecurityException: No permission to write APN settings](https://stackoverflow.com/questions/51440531/java-lang-securityexception-no-permission-to-write-apn-settings/51440864)

[解决android.permission.WRITE_APN_SETTINGS](https://www.cnblogs.com/zshengfei/p/5344519.html)

---

再一次限定了只能以System app的角色来申请该权限。

---


TODO：编译 Aosp 10 for pixel 3a 并提取证书和 framework/
