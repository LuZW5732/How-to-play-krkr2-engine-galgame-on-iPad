# How-to-play-krkr2-engine-galgame-on-iPad
如何在iPad上游玩krkr2引擎的galgame

本教程适用于iPadOS16/17/18，旧版系统方法更多，也可参考此方法操作。作者 路ZW

这个教程直接搬运自我撰写的同名pdf文件，未作任何更改。

可能需要用到的软/硬件：iPad、运行windows系统的电脑、爱思助手、AltStore、GARbro mod版、ScnEditorGUI、Sublime Text、WinHex、你下载的krkr版gal文件、同款gal的PC版文件

注：经过一段时间的游玩发现了几个问题，一是部分游戏可能无征兆闪退（？，二是部分游戏文件系统弹窗提示文件损坏从而卡死。我不是代码大佬，只能提醒各位多保存存档，以及迫不得已再重装游戏了。

由于游戏不是用完即抛的临时性文件，因此不建议使用爱思助手自带的自签名安装功能，自签名证书只有7天的时效，且爱思助手无法更新证书，所以我们在此使用可以更新证书的AltStore。

如果你之前在AppStore下载了xp3player，那么可以直接跳过有关AltStore的所有部分。

## 安装AltStore

首先请确保你的Windows系统电脑上安装了iTunes和iCloud，这是AltStore运行所必需的。

需要在你的电脑上安装AltServer，可以自行百度，或者访问我使用的下载链接：

https://tweak-box.com/altstore/#google_vignette

点击蓝色的“Download For Windows”按钮即可。

下载完成之后请解压得到的压缩包，不会解压请自觉关闭本教程，因为后面的教程只会更难。

打开setup.exe并跟随引导进行安装。

安装完成后会要求你重新启动电脑。

## 如何使用AltStore

点击任务栏右下角，会看到AltServer的图标（红框中）

![image](photos/photo1.png)

此时，打开iTunes，将你的iPad通过USB连接至电脑，iPad上会出现信任弹窗，点击“信任”并输入锁屏密码，然后可以看到iTunes软件界面左上角出现了iPad图标，点击iPad进入其总览界面，勾选“通过WIFI进行同步”（尚不清楚是否影响校园网流量，学生党不建议勾选），该功能可以使以后每次更新证书时不通过USB连接电脑即可实现更新。

左键点击任务栏中的AltServer图标，点击“Install AltStore”，然后会出现连接设备列表，点击你的iPad，此时会要求你提供你的AppleID和密码，部分账户还会要求提供二次验证的验证码（在iPad显示为想要在某地登录账户，点击允许，然后才会显示验证码），按要求输入。等待一段时间直到弹窗显示安装成功即可。

![image](photos/photo2.png)

iPadOS18目前尚不稳定，安装可能失败，多尝试几次即可。

安装完成后，打开iPad上的AltStore，会提示“未受信任的开发者”，此时打开iPad系统设置，点击通用-VPN与设备管理，此时会出现其中一个选项是你的AppleID邮箱，点击进入，然后点击蓝色字体的“信任”即可。

![image](photos/photo3.png)

## 通过AltStore安装xp3player

此时将xp3player的ipa安装包导入至iPad“文件”内，我这里提供Github源的xp3player下载链接：https://github.com/zeas2/Kirikiroid2/releases

如果受限于网络环境无法访问Github，也提供百度盘下载：https://pan.baidu.com/s/1rr_M_EhlaeeTCNMQuvojjg?pwd=0721

提取码0721

进入AltStore app，在底部导航栏点击My Apps，然后点击左上角+号，在弹出的页面中选择你刚刚导入的xp3player的ipa文件。

![image](photos/photo4.png)

安装可能失败，可多次重连USB或重新打开AltStore尝试。

已知iPadOS18测试版在每次通过AltStore安装软件成功后会重新要求验证证书，根据上文步骤前往系统设置重新信任即可。

## 通过爱思助手导入krkr游戏

**请先看完此部分和下一部分再进行操作**

网上大多会告诉你可以通过iPad内部文件共享功能自行导入至xp3player，但是这个方法早已随着iPadOS更新和作者停止维护而失效。

其实使用iTunes自带的文件共享功能也可以导入游戏，但是远不如爱思助手操作方便（并且不能删除文件）。

这里需要保持USB连接，打开爱思助手，会自动显示你的iPad综述界面，点击侧边栏的“应用游戏”，找到xp3player，点击右侧的“浏览”。

![image](photos/photo5.png)

此时会弹出新的界面，点击左侧的Documents，点击“导入”，将你的krkr版gal的整个文件夹传输进去。

![image](photos/photo6.png)

## 启动游戏（或者检测游戏状态）

通过爱思助手导入成功后，即可前往xp3player进行游玩了，一般通过点击data.xp3启动。

![image](photos/photo7.png)

如果点击之后成功启动了游戏，那么恭喜你，你可以退出本教程了，记得每6天连接电脑通过AltStore更新一次证书（点击My Apps界面内的Refresh All）。

如果点击之后软件闪退，或者卡住没有反应，那么你就需要继续往下看了。

本教程仅提供汉化组**系统弹窗导致的软件卡死**解决办法，其他问题请自行百度。

## 简易修复方法


方法一：

此办法仅限有缘人使用，至少我运行iPadOS18的iPad9无法使用此方法。

该方法来自于B站@超级玲音厨，BV1W142187ZM，感谢贡献。

多次点击三条杠中的“关于”，直到出现信息弹窗为止，然后就可以去启动游戏了。

方法二：

此方法限定特殊条件，至少我还没遇见过。来自于同视频的评论区，感谢贡献。

![image](photos/photo8.png)

方法三：

这个方法也是限定特殊条件，因为我解包完忘了把东西删掉（

我解包data.xp3的时候将startup.tjs直接扔在了游戏根目录里，这导致xp3player进入该文件夹的时候自动运行游戏，而这个游戏刚好有搬运组制作的系统弹窗，导致卡死。

解决方法就是直接删除这个startup.tjs，然后进入该文件夹就不会卡死了（）

## 游戏解包与读取修改

本部分以及往下所有内容均来自于B站 _@五娼会会长_，感谢贡献。

### 安装GARbro mod版

GARbro原作者已经停止维护，但是仍然有大佬在制作该软件的mod版，该软件提供了xp3解包封包加密等一系列支持，相当便利。

Github下载地址：https://github.com/crskycode/GARbro/releases

第三方百度盘链接：https://pan.baidu.com/s/1O26mJJGGF33YFp9oiwNYXA?pwd=0721

提取码：0721 

### 安装Sublime Text

该软件用于读取未加密tjs文件，界面美观，支持大部分编码格式。

官方下载地址：https://www.sublimetext.com/

第三方百度盘下载地址：https://pan.baidu.com/s/1NXVEoiNuIAnh6CBVmzQ49w?pwd=0721

提取码：0721 

该软件安装后需要汉化，具体步骤：

1.打开软件

2.按Ctrl+Shift+P调出快捷搜索栏

3.搜索Install

![image](photos/photo9.png)

4.点击Package Control：Install Package

5.等待一小会儿，重复1234步骤

6.搜索Chinese

7.点击第一个关联项，稍等片刻即可变为中文。

### 如何解包

打开GARbro，点击右上角文件-打开，找到你要解包的游戏文件夹，一般我们要找的文件名为data.xp3或者“运行游戏.xp3”，我们这里以操作流程较为简单的kr版《根本没有中之人！》为例。

![image](photos/photo10.png)

一般情况下xp3文件不会被加密，这里直接选择没有加密并确定。

![image](photos/photo11.png)

然后我们就能看到解包后的文件目录了。一般我们需要检查startup.tjs文件，点击该文件，右键点击提取，我建议在源目录新建文件夹用于放置提取的文件。

![image](photos/photo12.png)

![image](photos/photo13.png)

### 寻找系统弹窗相关文件并修改

提取出来之后，我们使用刚刚安装的Sublime Text打开startup.tjs，一般会看到如图所示界面。这里先对使用了普通tjs的游戏进行解释。

![image](photos/photo14.png)

但是根据在iPad尝试启动时显示的画面，系统弹窗显示的内容不在这里。

![image](photos/photo15.png)

如果这里打开时显示的是如图所示乱码（以kr版《与你相连的恋爱FLAG》为例），那么请往后查看“压缩tjs与tjs2”部分。

![image](photos/photo16.png)

根据第20行，该文件最后指向了游戏system文件夹中的Initialize.tjs，我们将其提取出来并打开，显示以下内容。

![image](photos/photo17.png)

现在我们看到第三行出现了System.inform("https://acg-moe.com","By 御宅同萌");，这便是我们要找的，直接将这行语句删除，保存文件并关闭。

### 文件封包与重新导入

现在我们回到GARbro，选中整个游戏目录提取出来。

![image](photos/photo18.png)

然后我们将修改后的Initialize.tjs替换掉system文件夹中的同名文件。

![image](photos/photo19.png)

现在打开GARbro，切换到提取后的游戏目录。

![image](photos/photo20.png)

选中所有文件，右键点击创建压缩文件

![image](photos/photo21.png)

在新弹出的窗口中勾选上“保持目录结构”。同时点击文件名右侧按钮，将创建位置指向到临时存放游戏文件的文件夹。

有一个有意思的bug，如果从startup.tjs开始选中所有文件，会导致GARbro右侧显示startup.tjs的预览，这造成压缩时提示该文件被占用从而封包失败。

解决办法：从bg文件夹开始从上往下选中所有文件即可。

![image](photos/photo22.png)

![image](photos/photo23.png)

封包完成后，需要关闭GARbro才能删除原先的“运行游戏.xp3”，然后用刚刚我们制作的文件来替换它，我这里用data.xp3来替换，它们的效果是一样的。

![image](photos/photo24.png)

此时可以删除临时存放文件，将游戏文件夹重新导入xp3player，因为先前我们已经导入过一次用于测试了，所以这次我们只需要用爱思助手删除原来的data.xp3，再将新的data.xp3文件导入即可。

![image](photos/photo25.png)

现在，我们在xp3player中启动data.xp3，就能正常游玩了。

![image](photos/photo26.png)

### 压缩tjs与tjs2

这里需要用到WinHex进行查看。

下载链接：https://pan.baidu.com/s/1ju8aWaRa_CqjUT9ggWC91Q?pwd=0721

提取码：0721 

我们用WinHex打开startup.tjs，发现右侧首行出现了TJS2100字样，这代表该文件实为tjs2，否则就是压缩tjs。

![image](photos/photo27.png)

压缩tjs的处理方法需要使用KirikiriDescrambler，将tjs文件拖动到KirikiriDescrambler.exe打开，不用在压缩回去。

Github下载链接：https://github.com/arcusmaximus/KirikiriTools/releases/tag/1.7

我目前还没有遇到使用压缩tjs的galgame，且我的win11不知为何无法运行这个软件，所以在此不作更多解释。

在确定为tjs2文件后，我们需要用其他的软件对其进行修改。

这里 *@五娼会会长*大佬给出了两款可以用于修改的软件，分别是KrKrzSceneManager和SacanaWrapper，第二款软件由于同上原因我无法运行，所以只能对第一款软件进行讲解。这两款软件修改形式相同，只不过第二款会以txt文件形式提取出来，便于你修改。

第二款软件使用方法：把tjs拖至StringTool.exe上即可，封回去的话，选中原始tjs和解出来的txt，一起拖至StringTool.exe上，生成一个xxx.tjs.new，把new去掉即可。

现在讲第一款软件KrKrzSceneManager的用法。

Github下载链接：https://github.com/marcussacana/KrKrZSceneManager/releases/tag/1.0.31

第三方百度盘链接：https://pan.baidu.com/s/11nqTO5hSaYctUhwrUY0CTQ?pwd=0721

提取码：0721 

打开ScnEditorGUI.exe，显示如下画面。

![image](photos/photo28.png)

右键调出菜单，选择TJS2-Open

![image](photos/photo29.png)

选择打开startup.tjs，显示如下画面。

![image](photos/photo30.png)

这个游戏的startup.tjs也引导我们去system/Initialize.tjs，再打开Initialize.tjs，现在出现了我们要找的内容……（这里以较难修改的小鸟游 晓大佬制作的kr版为例）

![image](photos/photo31.png)

这种情况修改起来非常麻烦，因此我们转而使用PC原版的相同文件进行比较。

![image](photos/photo32.png)

这里能发现两个文件存在极大不同，但是却可以直接拿PC原版的Initialize.tjs文件替换krkr版的相同文件。直接替换后重新封包导入即可游玩，但是可能会影响性能和部分功能实现。

![image](photos/photo33.png)

现在讲其他情况，以妹抱为例。

将PC原版的startup.tjs与kr版文件进行对比，发现两者最后指向了不同的文件。

![image](photos/photo34.png)

Krkr版最后指向了startup2.tjs，接下来我们查看startup2.tjs，于是找到了源头。

![image](photos/photo35.png)

解决办法也很简单，直接修改语句重新指向Initialize.tjs或者拿原版tjs替换都可以，然后重新封包导入即可。


## 参考文献：

1.ios端krkr模拟器弹窗卡死问题解决办法 作者@五娼会会长https://www.bilibili.com/read/cv21331113/?spm_id_from=333.999.0.0

2.Krkr引擎工具合集（一）——解包封包 作者@五娼会会长https://www.bilibili.com/read/cv20898536/?spm_id_from=333.999.0.0

3.Krkr引擎工具合集（二）——脚本、编码、文字 作者@五娼会会长https://www.bilibili.com/read/cv21072666/

有遇到不懂的可以查看这些B站专栏，对许多问题都给出了解释，同时在xp3解封包等方面讲述得更为详细。


以上就是本教程的全部了，祝大家玩的开心。

——路ZW
