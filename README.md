# Triple C Educational Program Web Fundamental Final Assignment  

## Purpose of this assignment:  
- 此项目作为Web Fundamental组的结业项目，可以让你很好地锻炼已经学过的web前端开发的基础知识。  
- 如果想继续参加React项目组的学习，我们会以此项目的完成情况作为面试的重要参考标准之一。  
- 如果想参加Triple C在后续学期有小概率提供的```HTML, CSS, JS, Jquery```相关的Web项目，完成了此Assignment的你会有绝对的优先权。  

## 开始之前：  
- 请确保你已经熟悉```HTML/CSS/JS```, ```Jquery``` 以及 ```ajax``` 。  
- 请确保你对**什么是API**以及**如何从一个API获取数据**有基础了解。  
- 即使到最后没有完整/完美地完成这个assignment，你依然具有参加Triple C后续面试/项目的资格，且此assignment在Triple C的后续面试中只会起到**extra credit**的作用，i.e. assignment即使完成情况不佳也不会对你的面试产生任何影响。  

## Assignment简介：  
本次项目分为三个部分:  
**1. 使用```HTML和CSS```制作静态网页:**  
![pic1.png](https://i.loli.net/2021/01/06/N9l3GIyCcYg1awq.png)  
<br/>
<br/>

**2. 调取任意公共API，完成一个简单的web app（后面会有详细说明）：**  
![pic1.png](https://i.loli.net/2021/01/06/rEqFUb8xYHmZMhp.png)  
<br/>
<br/>

**3. 完成一个个人网页（后面会有详细说明）：**  
![pic3.png](https://i.loli.net/2021/01/06/XQFcxgCYW3p1za7.png)   
<br/>
<br/>

## 具体说明：  
### 1. 静态网页：
[在此处查看WireFrame设计图](https://www.figma.com/file/x2din21LcGqaP7zYyShSzN/TripleC_Summer20_HTML?node-id=0%3A1)  
打开Figma页面之后，点击某一个部件，然后点击右边的```code```就能看到对应的CSS代码实现  
部件的大小（长宽）请根据你的屏幕尺寸做出自适应
<br />  
![pic7.png](https://i.loli.net/2021/01/06/a2lSTIVs6L1BNGY.png)  
**!注意** 此处的CSS代码为Figma自动生成，只是为了简化你的CSS调试流程，并不是为了让你全部照抄。  
你可能注意到了，Figma生成的几乎所有CSS代码都在用 ```position: absolute``` 进行定位。如果你的页面上也全部用的都是 ```position: abosolute``` 定位，那么你的这一项assignment将被直接记零分**。   
（原因：如果所有部件都是 ```position: abosolute``` ，那么我们做的网页就不能自动适应不同尺寸的分辨率。那写HTML和CSS还有什么意义呢？不如直接放一张固定大小的svg算了）  
<br />
  
**细节说明:**  
- 你写的页面只需要跟Figma上的设计图**布局一样**，(i.e. card, navigation bar这些部件在它该在的地方），不需要在意功能  
- 页面需要**占满**你的屏幕。你在Figma里面看到的```Page-1```这个Frame就是你的屏幕。
- 上面含有```CSE11```的那个框框是个输入框，要可以输入文字  
- 输入框右边的两个是```button```，点击之后不需要发生任何事件
- 再往右的sign in是```link```，点击之后任意跳转到哪都行
- 左边```Top Departments```那一竖条是一个```unordered list```
- 最下面```Show All```和```Show More```是```button```，点击之后不需要发生任何事件
- 最上面的navigation bar需要贴紧屏幕最上面，同时需要在**任何屏幕尺寸**下都能占满整个屏幕的宽度
- 页面的颜色，有些部件的```border-radius```等，你都可以在Figma里直接获取到，不用自己去调

**extra credit**  
- 你可能看到了这个设计图长得非常丑。尝试用```bootstrap```里的相应部件替换页面上的部件
- 让页面在不同屏幕尺寸下有更强的适应性。比如：在手机这一类屏幕宽度很小的设备上，右边的Card每一排只显示一张，而不是两张；在手机屏幕尺寸下，左边的```Top Departments```这个list，只有在点击某个按钮时才会出现  
<br />
<br />

### 2. web app：  
在这个部分，你会需要更多的创造力。  
**要求**： 自己选择任意一个API，用ajax调用这个API，然后在你的网页上展示从这个API获取到的数据。  

**例子1：**   
从 [https://openweathermap.org/api](https://openweathermap.org/api) 获取天气数据制作的天气app  
![pic1.png](https://i.loli.net/2021/01/06/rEqFUb8xYHmZMhp.png)  
See a demo here: [https://weather.ucsdtriplec.org](https://weather.ucsdtriplec.org)  
如果你也想做类似的项目，那么你不用做的跟这个demo一样复杂。  
你需要做的可以只有：
- 让用户输入一个城市名字，然后展示这个城市现在的天气数据
- 或者更简单的，直接展示全球著名城市的天气数据  
<br />
<br />

**例子2：**  
从 [https://earthquake.usgs.gov/fdsnws/event/1/](https://earthquake.usgs.gov/fdsnws/event/1/) 获取全球地震数据制作的地震监测app。  
<img src="https://i.loli.net/2021/01/06/8WrfuhMCAVNcl9p.png" width="250px">  
[更详细的项目介绍请点击这里](https://github.com/dekunma/EarthquakeMonitor-ReactNative)  
  
**这个例子并不是在说你可以做一个手机端的app**  
这个例子虽然是一个手机端的项目，但你也完全可以用你学到的知识把它做成网页端。  
总体逻辑都是一样的：从API获取数据，然后把获取到的JSON file处理之后，再在屏幕上展示出来。
如果你也想做类似的项目，同样地，你不用做得跟这个demo一样复杂。
<br />
<br />

**从哪里找API？：** 
- 你可以看看 [https://github.com/TonnyL/Awesome_APIs/blob/master/README-zh.md](https://github.com/TonnyL/Awesome_APIs/blob/master/README-zh.md) 提供的一些非常不错的公共API。
- 这其中很多API会需要你点进去之后阅读这个API的documentation。这个过程很让人头疼，但这是前端开发者必须经历的。
- 可以直接谷歌搜索xxx API
<br />
<br />

**其他brain storm：**
- 想一想你对什么感兴趣
- 如果你对时事感兴趣，那你可以调用某个新闻网站的API，然后做一个展示新闻的网页
- 如果你对足球感兴趣，我记得你可以找到历年世界杯数据的API。你可以做一个网页来筛选，展示相关数据
- 如果你对炉石传说感兴趣，那我记得应该有炉石卡牌的API。你可以做一个网页来展示/搜索炉石卡牌
<br />
<br />

**细节说明：**  
- 在这个项目中，你**必须**至少从一个API获取数据，并以某种方式使用/展示数据（如果你看到这里了依然不太确定我在讲什么，可以重新去学习ajax）。  
- 你可以参考别人的代码，但你必须理解你抄的代码。同时大段的代码引用(>=30 lines) 必须注释代码出处。同时你**不可以**整个项目都完全白嫖别人的代码。
- 花时间想想你想用什么API来展示什么样的数据。如果实在想不出来，那么我举的前两个例子（天气和地震API）也是可以勉强接受的。 
- 你可以使用包括但不限于```BootStrap```, ```semantic ui```的任意UI库来完成这个assignment
<br />
<br />

### 3. 个人网页：  
我们对这个页面**没有任何具体要求**  
用你在前两个页面里学到的技能做一个自己的个人介绍页面就可以  

实在不知道做什么可以参考 [li-mao.net](https://li-mao.net) （Triple C历届社长李懋的个人网站）  
以及 [www.dekun.me](https://www.dekun.me) (很久没更新了)  
![Screenshot 2021-01-06 113944 1.png](https://i.loli.net/2021/01/06/EiILeuUVbBkcRal.png)  

**brain storm ideas：**
你可以展示这些信息：
- 你的名字
- 联系方式
- 教育经历
- 项目经历
- 上过的课
- 个人爱好等  
<br />
<br />

## 项目完成之后  
请新建一个**private**的Github repo，将代码上传至这个repo，并邀请账号```dekunma```加入   
或直接将代码打包发至```William@dekun.me```  
我们会在完成对你代码的简单评估之后，针对你做的项目，对你进行面试  
**如果你的完成情况很好，并且你希望的话，我可以免费部署你的项目。（这样你以后给别人分享项目的时候可以直接用URL)**
<br />
<br />

## 关于Violation of Academic Integrity
**零容忍。**  
在本次项目里你可以调用外部库，或参考别人的代码  
但如果全部直接白嫖别人的代码，你会直接失去参加Triple C任何后续面试的资格  
我们都不希望这种事情发生  
<br />
<br />

## Frequently asked questions: 
- Q: 这个assignment什么时候due？  
    A: 没有due date。这个项目只是为了让你练习学过的技能，并为你后续参加Triple C的面试/项目添加筹码。虽然没有due date很难做成事，但自己掌握自己的学习节奏和 学业/休息/其他事情的平衡 也是非常重要的能力。  
      
- Q：我可以选择不做这个assignment吗？  
    A：可以。

- Q：如果我直接不做这个assignment，Triple C会对我产生不良印象吗？  
    A：不会。考虑到线上学习的缘故，我们在这几个学期经历了莫大的挑战，educationa program的开展也进行了非常多无可奈何的调整。所以如果你觉得这次的的学习体验不佳，也可以选择不做这个assignment。但Triple C欢迎你在掌握了其他技术栈之后，重新报名面试，加入项目组。

- Q：如果我完成了这个assignment，我可以直接加入生产项目组吗？  
    A：需要看情况决定。如果这个assignment完成的人数多，质量高，并且完成assignment的人数达到了开展新生产项目的最低标准（~4人），我们会考虑为你们专门组建一个项目组，大家直接开始上手做项目。
<br />
<br />

## 其他任何问题
请随时写邮件至 ```William@dekun.me``` 提问  
或直接在群里@我 或私戳我
