# 物联网241 陈娄昊
## 与Win11斗智斗勇---艰辛git之路 
>*<font color="blue">*可能对于各位高手来说，git的使用易于反掌，但对于我这个小萌新嘛*。</font>

# 太痛力 

  
**as we all know 啊，** 从来没有用过shell的本小萌新呢，虽然一开始有点蒙哈   **但是** 一开始看到类似
  
```
git init
git add.
git commit -m "first commit"
  
```
的代码，跟着攻略走还是很清楚他的意思的。
### 万万没想到啊，问题出在了俺的Win11上
怎么回事呢？
- [x] (心路历程ing)
。
。
。
## git add 时 显示电脑有权限操作的用户和目前用户不一致
```
error:the user should be XXX
but now the user is YYY
``` 
 <font color="green">点名表扬</font>win11的安全设置，非常“安全”的设计，不但防住了病毒，差点没给我送走
  
- [x] （解决方法） 
绞尽脑汁 包括但不限于进行了以下尝试：
- 1 给与目前用户权限   然后电脑哥们自己给我改回来了
- 2 修改那个有权限的用户的权限，然后电脑不让改 。。。
- 3   重启 直接试图用管理员身份运行git 希望bush出奇迹 然后电脑无视了我 ...
- 4 怀疑 stydio code是否有问题,干净利落刷新--卸载重装 ，然并软 
- 5 阅读win11手册，在几千字的手册中，并没找到符合的那一条
*怎么就搞不出来？？事实上，后来我才知道，以我浅薄的知识，妄想取得win1的完全掌控，是不可能滴。*
# 在关闭了**7**个csdn,**11**个百度，4个b站视频后
我陷入了沉思。
是的，以前有过一次，我试图关掉每次必弹出来的请求关掉权限弹窗，在bilibili上得到了求解。
但是这种事情，我还第一次见。
  
## 针对win1安全系统做的任何努力都失去了意义，我只能顺从他了
  
 <font color="blac">我把所有的打开的相关软件全都用管理员模式再次打开，把早被我关掉的window安全管家再次打开了，</font> 
## <font color="red">芜湖！ 成了！！！</font> 
  
> 试成功以后，我试着用 减法原则  一个一个排查到底哪些开管理就行了，尽管我不清楚原理，但我总归试出来了：
git 和 code 一起开，同时满足window 管家激活，权限维持初始设置，不能修改权限，然后就可以了。
至于其他点小问题夜出过一些，不过不严重，后面就轻松拿下了 
```
error:permission denied   没权限
```
```
not a git repository     不是git仓库   
  
```
  
```
nothing to commit,working tree clean   工作树干净 没传成功
  
```
一个没落下，不过小查一波。全都拿下。
  
看着现在运行良好的git，我心里还是很开心的，不管怎么样，终于是搞完了。
  