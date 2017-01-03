Google  Service Unity Plugin
==============================
Google Service Unity Plugin is a Unity Plugin For Google Service.Include Google Admob Unity,Firebase Analytic Unity,Google Game API Unity. Login,Achievement,Leaderboard,Event,Quest,Snapshot,RealTimePlayGame,TurnbasedPlayGame API are supported and easy to use with c# or js.

## Unity Plugin Wiki and Documentation
* [Unity Admob API](https://github.com/unity-plugins/google-play-game-service-unity-plugin/wiki/Admob-Unity-Plugin-API)
* [Unity Firebase Analytic API](https://github.com/unity-plugins/google-play-game-service-unity-plugin/wiki/Firebase-Analytic-Unity-Plugin-API)
* [Unity Google Game API](https://github.com/unity-plugins/google-play-game-service-unity-plugin/wiki/Unity-Google-Game-API)
* [Unity Admob Tutorial](https://github.com/unity-plugins/google-play-game-service-unity-plugin/wiki/Admob-Unity-Plugin--Tutorial)
* [Unity Firebase Analytic Tutorial](https://github.com/unity-plugins/google-play-game-service-unity-plugin/wiki/Firebase-Analytic-Unity-Plugin-Tutorial)
* [Unity Play Game Service Tutorial](https://github.com/unity-plugins/google-play-game-service-unity-plugin/wiki/google--Play-Game-Service-unity-plugin-Tutorial)
* [Firebase Remote config and log](https://github.com/unity-plugins/google-play-game-service-unity-plugin/wiki/Firebase---Service--Remote-Config-and-Log)

## Quick Start

### Installation Google Play Game Service Unity Plugin
1. Open your project in the Unity editor.
2. Navigate to **Assets -> Import Package -> Custom Package**.
3. Select the google_service_unity_plugin.unitypackage file.
4. Import all of the files for the plugins by selecting **Import**. Make sure
   to check for any conflicts with files.playgamedemo.cs and game.unity is demo file  can be ignored.
5. replace all "com.google.demo" with your app package id in AndroidManifest.xml
6. replace app_id content with your google play game id,replace google_app_id content with your google firebase app id in ids.xml


### Show Admob Ads in Unity game

	using admob;
	Admob.Instance().initAdmob("ca-app-pub-3940256099942544/2934735716", "ca-app-pub-3940256099942544/4411468910");
	Admob.Instance().showBannerRelative(AdSize.Banner, AdPosition.BOTTOM_CENTER, 30, "defaultBanner");

just 2 line code,admob banner will been shown on screen.for more usage  [Unity Admob Tutorial](https://github.com/unity-plugins/google-play-game-service-unity-plugin/wiki/Admob-Unity-Plugin--Tutorial)

### Analytic Unity game with firebase Analytic

	using google.service.game;
	FirebaseAnalytic.Instance().logEvent("appstart", "{\"time\":\"112222\",\"name\":\"demouser\"}");

Log Event with Firebase Analytic.For more usage about Firebase Analytic Unity  [Unity Firebase Analytic Tutorial](https://github.com/unity-plugins/google-play-game-service-unity-plugin/wiki/Firebase-Analytic-Unity-Plugin-Tutorial)

###  Using Google Play Game Achievements and Leaderboards in Unity game

1. Login with google play service
```
	using google.service.game;
	GoogleGame.Instance().login (true, false);
```
2. You can call google play game api after login success such as show Leaderboards with default UI
```
	GoogleGame.Instance().showLeaderboards();
```
3. Show Google play game Achievements with default UI
```
	GoogleGame.Instance().showAchievements();
```
4.Fore more usage about google play game service in unity [Unity Google Play Game  Tutorial](https://github.com/unity-plugins/google-play-game-service-unity-plugin/wiki/google--Play-Game-Service-unity-plugin-Tutorial)    
     
    
![ScreenShot](https://raw.githubusercontent.com/unity-plugins/google-play-game-service-unity-plugin/master/screen.png) 

Project Home   https://github.com/unity-plugins/google-play-game-service-unity-plugin/
