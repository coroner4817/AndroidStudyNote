# AndroidStudyNote

My Android tricks notes (pages are for 第一行代码)

1, use BaseActivity p77

2, use ActivityColletor manage activities p78

3, best way to start activity p80 actionStart

4, layout_weight=1; layout_width=0 p110 111

5, use <include layout=""/> p123

6, improve ListView p133

7, use nine patch to resize image p141

8, use <fragment name=""/> in <frameLayout/> in xml p175
   don't need fragmentManager, dynamic load fragment

9, different screen use diff layout folder p184

10, BroadCast to inform others any changes in your app
    System level:
    Standard BroadCast p197
    Order BroadCast p199
    App level:
    Local BroadCast p203

11, file save to default folder and will be delete when uninstall p221
    use DDMS to see the file in phone p224

12，SQLite p239
    use adb to check database p244 p251
    SQLite transaction to stop database execution p261
    Best way to update database p263

13, ContentResolver and ContentProvider
    use ContentResolver to load system data, such as contacts p269
    create own ContentProvider and exposed to other apps p276
    Check all ContentProvider in device adb shell dumpsys | grep Provider{
    Share database between apps p281

14, analog SMS RX SX and Stop p308

15, use camera take pic and crop p322
    select image from gallery p327

16, play audio and video p332 p336

17, Thread
    Update the UI in the child thread p346
    AsyncTask(same as BackgroundWorker in C#) p348

18, Service p353
    Service communicate with Activity p359
    use startService, stopService then service is not control by the activity
    use binService and unbindService to start service then the service can be controlled by the activity but will service die when unbind
    so use startService first then bind it
    service can only be started once
    use front-end Service p364
    service standard version(use thread) and stopSelf() p367
    or use IntentService when doing some heavy task in service. It will automatically stop when task finished p368
    Like a service manager, terminal useless service to avoid traffic in Main UI
    wake up service in period p371

19, Web-based development p377
    ...

20, XML & JSON p388
    ...

21, GPS based app p409
    ...

22, phone sensor app p439
    light p439
    accelerate p443
    direction p446

23, ApplicationContext never die
    Activity Context die with the activity.onDestory()

24, use Intent to transmit object
    Serializable p459
    Parcelable(faster) p461

25, UnitTest p468
    Android studio level to control all the files in the project
    a programmable debugger


--------------------------------------------------------------------------------


Android project

1, simple chatApp example p145
2, fragment ex p175
3, force logout (Local BroadCast) p205
4, Share database between apps p281
5, Cool Weather p476 ***
6, Timber music player
    https://github.com/naman14/Timber
7, PhotoNoter
    https://github.com/yydcdut/PhotoNoter
8, NBAPlus
    https://github.com/SilenceDut/NBAPlus ***
9, OpenSource Analysis
    https://github.com/android-cn/android-open-project-analysis


--------------------------------------------------------------------------------


GitHub UI repo
1, Summary
  1, https://github.com/kesenhoo/android-open-project
  2, https://github.com/wasabeef/awesome-android-ui

2, overall structure
  1，https://github.com/florent37/MaterialViewPager
  2，https://github.com/kot32go/KSimpleLibrary
  3，https://github.com/tosslife/FoldingTabBar.Android
  4，https://github.com/Yalantis/Side-Menu.Android
  5，https://github.com/android-cjj/Persei.android

3, Image
  1, gallery
    https://github.com/pengjianbo/GalleryFinal

4, ListView
  1, https://github.com/nhaarman/ListViewAnimations

5, SwipeRefresh
  1, https://github.com/ashqal/ChromeLikeSwipeLayout

6, Animation
  1, https://github.com/lgvalle/Material-Animations

7, SoundControl
  1, https://github.com/RSenApps/Commandr-Android

8, Drawer
  1, https://github.com/mxn21/FlowingDrawer

9, Service
  1, https://github.com/andyiac/PermanentService


--------------------------------------------------------------------------------


Some online notes
1, [Gradle for Android](http://gold.xitu.io/entry/56946cfa60b2b80a9d1c173f)
2, [Android性能优化典范](http://geek.csdn.net/news/detail/50692)
3, [Android退出应用最优雅的方式](http://android.jobbole.com/82335/)
4, [android开发小技巧积累/](http://souly.cn/%E6%8A%80%E6%9C%AF%E5%8D%9A%E6%96%87/2015/12/16/android%E5%BC%80%E5%8F%91%E5%B0%8F%E6%8A%80%E5%B7%A7%E7%A7%AF%E7%B4%AF/?utm_source=tuicool&utm_medium=referral)
5, [Android小技巧(1)](http://android.jobbole.com/80645/)
6, [安卓开发的小技巧（1)](http://android.jobbole.com/82206/)
7, [100套最新UI PSD素材打包下载](http://www.uisdc.com/2016-100-daysui-psd)
8, [git分支最佳实践](http://www.kuqin.com/shuoit/20141210/343783.html)
