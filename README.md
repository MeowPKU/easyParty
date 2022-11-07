# 一、简介
一个很棒的前端设计，基于html，css和javascript，旨在使得人们之间的聚会变得简单、快乐和有趣。

# 二、小组信息
## 1.小组队名
MeowPKU(Make Each One Warm in PKU)

## 2.成员信息
|职务|姓名|学号|年级|分工|
|:-:|:-:|:-:|:-:|:-:|
|组长|肖萧|2100016653|21级|撰写代码、监督项目实施、对项目进行版本维护|
|组员一|税远志|2100016640|21级|玩|
|组员二|罗泽阳|2100016650|21级|摆（x|
|组员三|果果|2000093014|20级||
|组员四|王涵|2100016625|21级|乐|

# 三、网站项目定义
## 1.网站名称、logo
![](./.demo/logo.png)

## 2.设计说明
### a)情境
#### i.情境描述
在学校里，想要或需要进行多人活动时，同学们可能找不到一起的搭档、伙伴。偌大的学校里，想要进行如爬山、桌游、看电影、一起听歌等活动，我们一般只能邀约熟悉的若干朋友，但常常难以做到意愿统一；如果去树洞发布邀约帖子，由于树洞人群在线的人数动态变化大和树洞繁杂的消息，邀约很容易石沉大海，很难被真正有相同兴趣的同学看见。

目标情景：

一方面，本网站帮助同学们发布约人邀请，这一邀请帖子可以设置时间、地点、人数范围、性别、用户备注。
网站的邀约展示页面可以展示最新发布的邀约帖，也可以根据邀约属性划分为不同的类型区域，如桌游类、电影类、外出游玩类等区域。
用户可以自己给发送的帖子贴标签，从而使它进入对应的类型区域，让有相关兴趣的人更方便看到；同时，网站也具有分析帖子属性关键词功能，自动将无tag帖子放入对应区域。
根据用户发送的帖子的tag，系统会自动为用户进行用户画像。之后用户打开网页的类型区域版，会首先展示用户爱好的类型。
帖子有评论区，其他同学可以了解详细情况。接收邀约的同学会被拉入与发起者共有的群组，群组人数会在评论区自动动态展示更新，满员后自动关闭评论区（可后续论证其合理性）。
如果帖子没有得到回复，网站会记录用户的邀约受挫记录，在其他用户发布相关贴子时进行提示。
邀约可以分短期邀约和长期邀约、临时起意和长期兴趣，短期、临时的邀约过一定时间后会被系统清除。

另一方面，网站有分享板块，成功组队玩耍后，用户可以在此分享照片、视频、文字。
用户有信誉积分，爽约、发起不良邀约后会扣分，给予一定处罚。经常准时赴约和邀约的人会加分，高分段用户将被给予“聚趴达人”称号。
网站有玩耍推荐网页。管理员首先负责更新相关玩物、景点推荐，如新的剧本杀、餐馆、某处景点。另一方面，聚趴达人可以申请负责相关推荐板块的管理，管理每位同学上传的推荐语。

#### ii.故事板

### b)用户
#### i.用户调研报告
##### 问卷

(此处插入2-7题图片（可选）及分析)

![](./.demo/statistical/T9.jpg)

从问卷结果来看，我们的用户更习惯于在线上发出邀约（如通过微信、QQ等社交平台），更倾向于邀请相熟的朋友（如通过线下面对面邀请）。结合我们访谈得到的信息以及现实生活中的经验，之所以会有这样的特点可能是在线上与人交流会比线下交流更放得开、没那么尴尬，同时线上交流能够随时随地进行非常便利，另外，大家在社交上普遍防范意识比较强，对陌生人的戒备心比较重，也认为跟陌生人交流会比跟熟人交流更容易尴尬，因此在邀约时更倾向于邀请相熟的朋友。

![](./.demo/statistical/T10.jpg)

从问卷结果来看，我们的用户在需求上呈现多样化的特点，娱乐型需求（如一起吃饭、一起逛逛、一起看电影）和学习型需求（如一起自习）都占有较大的比例，同时，线下活动（如一起吃饭、一起逛逛）的邀约需求要远高于线上活动（如一起听歌、一起打游戏）的邀约需求。这也为我们设计网站的相关版面提供了参考（如按照活动类型对发布在平台上的邀约进行分面展示、根据用户的选择提供跟踪活动等相关措施以尽可能保障用户安全）。

![](./.demo/statistical/T11.jpg)

从问卷结果来看，我们的用户绝大部分都想要继续与一起进行某一活动的其他用户继续保持朋友关系。这也为我们的网站功能设计提供参考（如在注册时绑定用户的联系方式，由用户按照自身意愿决定是否公开）。

![](./.demo/statistical/crossAnalysis1.jpg)
![](./.demo/statistical/crossAnalysis2.jpg)

从交叉分析结果来看，性格偏内向的用户比性格偏外向的用户会更容易认为主动发出邀约是一件困难的事情，也会更期待自己约到的人是比较外向的人。基于这一特点，我们考虑根据一定的规则为用户颁发相应的头衔（如社交达人），为这一类有期望的用户提供参考。

![](./.demo/statistical/T13.jpg)
![](./.demo/statistical/T14.jpg)

从问卷结果来看，我们的用户对各类推荐信息的需求都比较强，同时也希望推荐信息中除地点外包含具体的路线导航、预估人均花费等详细信息。

在本次问卷中，部分用户还提出了其他非常具有参考价值的建议，比如希望后台对所有用户进行实名（如绑定学号、真实姓名等）、跟踪线下活动（如到达预定时间时提醒用户进行“活动已结束，我已安全离开”的结束确认）防止动机不纯者给其他用户带来麻烦甚至造成伤害，同时也要注重保护用户隐私安全，还有希望推荐信息中的路线更多样化，同时路线的推荐也要贴合学生用户的身份（可能搭乘公共交通工具出行较多）等。
##### 访谈
（访谈报告以附件形式发送）
##### 用户划分
|                       |第一类人群用户（偏外向型） |第二类人群用户（有时外向有时内向型）   |第三类人群用户（偏内向型） |
|:----------------------|:--------------------------|:--------------------------------------|:--------------------------|
|基本属性               |人数较少；性别比例较为均衡 |人数较多；性别比例较为均衡             |人数较少；性别比例较为均衡 |
|行为习惯               |1. 认为主动邀约没那么困难；2. 比另外两类用户更愿意主动邀约；3. 比另外两类用户更愿意线下面对面发出邀约，出于对便利性的考量线上发出邀约也很多；4. 会使用树洞/BBS面向不熟的人发出邀约；5. 邀约类型广泛|1. 认为主动邀约较难；2. 倾向于等待被约；3. 更习惯线上发出邀约；4. 会使用树洞/BBS面向不熟悉的人发出邀约，但更担心安全性问题（如是否会遇到奇怪的人）；5. 邀约类型广泛|1. 认为主动邀约很难；2. 倾向于等待被约；3. 更习惯使用线上平台、比有时外向有时内向的人更倾向于线下向熟人发出邀约；4. 会使用树洞/BBS向不熟悉的人发出邀约，但更担心交流时的尴尬心理；5.	邀约类型广泛|
|对网站的关注点（推测） |推荐信息的丰富性、网站用户数量|用户隐私安全、人身财产安全保障|站内匿名性聊天室|

#### ii.典型用户画像
|属性|描述|
|:--:|:----------:|
|昵称|吃午饭等晚饭|
|性别|女|
|年龄|19岁|
|学历|在校本科生|
|互联网经验|能够熟练上网；主要进行通信交流、游戏娱乐、信息浏览、网络购物等活动；每天上网时间（PC端和移动端）在5小时以上；各类社交软件使用最多；|
|兴趣爱好|摄影、打游戏|
|人物简介|这位同学是一名大二在校学生，今年19岁，经常跟朋友相约去一些热门地点拍照，休闲时也会约朋友一起打游戏或者是看电竞比赛，在校内也时常约朋友一起逛逛校园拍拍照或是品尝新出的菜品。|
|用户行为|（形式）大多通过微信/QQ或是面对面线下的形式，倾向于线上邀请相熟的朋友；（频次）大约每个月约朋友出校游玩两到三次，大约每周在校内约朋友逛校园或品尝新菜品等两到三次，大约每两周约朋友看一次电竞比赛，大约每两周约朋友打一次游戏|
|烦恼经验|时常遇到朋友们没空、邀请被拒的情况，由于没有便捷渠道能够在校内约到其他兴趣相投的人一起去拍照游玩等，一些行程只好取消。|
|用户态度和观点|1. 线上发出邀约的原因：方便、能有效避免尴尬；2. 对约到的人的期待：兴趣相投、外向、准时守约等；3. 偏好的信息类型：校内外的美食、适合拍照游玩的宝藏景点、游戏相关资讯；4. 对向校内不认识的同学发出邀约的担心：性格不好相处、没有共同话题、爽约、动机不纯等|



### c)过程
#### i.接触点
需求、账户、个性化、浏览、邀约、搜寻、评论、应约、联系、打卡、分享、反馈、举报

#### ii.各接触点的用户任务
1. 需求

**用户任务：** 用户产生想要同其他人聚会的想法，抑或是在闲散时间想要进行诸如踏青、自习、参观等有意义的活动。一旦用户产生了诸如此类的想法同时又苦于难以找到志同道合的伙伴时，我们的产品就能对应于用户的需求。

**用户感受：** 用户苦于找不到和他一起进行某项活动的朋友，内心感到焦躁、不安和苦恼。

2. 账户

**用户任务：** 用户在我们的网站上注册账户或者是登陆账户，便于平台辨识、管理和服务用户。用户必须经过注册并登陆成功后才能接受平台提供的各种服务。

**用户感受：** 在注册阶段，长期的注册失败会让用户感到受挫和不耐烦。在登陆阶段，用户会因为一直登陆不上而感到焦急和恼火。

3. 个性化

**用户任务：** 用户修改个人信息，管理个人空间，整理自己的评论、帖子，以便其他用户更好地了解自己，向外界展示自己的良好形象，平台参考用户的个人信息对其进行有针对性的个性化服务。

**用户感受：** 用户修改自己的个人信息，如果修改过程过于繁琐，会引起用户的反感和不适，对于用户想修改而又不能修改的内容，如果呈现给用户会使用户感到焦急，对隐私和敏感信息会产生担忧。

4. 浏览

**用户任务：** 用户进入了网页，进行网页冲浪并获取用户想要的信息，包括新发布的邀约帖子、关于某一帖子的他人评论、其他人的活动分享、热门打卡景点推荐、热门游戏活动的测评等信息。

**用户感受：** 面对海量的信息，用户只关心他所想要的信息，如果不进行有效的信息筛选会使用户感到茫然和无所适从，用户拿到了想要的信息后应当要能确定信息的真实性、可靠性和失效性。

5. 邀约

**用户任务：** 用户拥有明确的活动目标但是缺乏和他一起开展活动的朋友，希望召集一批可以和他一起进行活动的伙伴，此时他可以发起邀约帖子，明确参与要求、活动时间和活动地点，在平台上召唤有条件且有意愿参与活动的朋友们。

**用户感受：** 用户拥有明确的活动目标，但可能对于活动的具体方式、时间、地点等细节以及如何明确表达自己的需求难以确定，因而感到困惑和迷茫。当用户发送了一份邀约帖子后，他会关心帖子的召集进度和关于帖子的各种反馈。

6. 搜寻：

**用户任务：** 输入活动名称，搜索有关帖子。如果有，会具体了解后考虑是否加入；如果没有，可能就此作罢或者自己发起此活动的邀约帖。

**用户感受：** 用户有进行某项活动的意向，但没有共同参与的同伴，内心有点苦恼

7. 评论

**用户任务：** 用户找到了自己感兴趣的活动邀约帖后，可以在评论区评论，一方面可以向邀约发起者具体了解活动相关信息，另一方面可以以旁人的角度单纯发表自己的想法；同时用户在资讯板块下也可以进行评论

**用户感受：** 没有同伴的孤独、迷茫、苦恼情绪减少，对活动提起兴趣，在不断了解中好奇心得到满足，心情转向和乐；在资讯板块下，用户见到他人、官方对相关活动的评价，如果是正向的，会更加渴望参与相关活动

8. 应约

**用户任务：**  用户了解之后认识到，某帖子下的活动及其参与者与自己的想法较为类似，于是进入发起者的活动群组，共同构成一个活动队伍

**用户感受：** 由不断了解时的和乐，转向和其他人形成活动队伍之后的喜悦、期待

9. 联系

**用户任务：** 活动开始前和进行过程中，活动群组内成员相互联系，获得共同的活动体验

**用户感受：** 成员之间的熟悉度不断加深，如果相处得融洽，会自得其乐，乐在其中；如果相处得不好，会讨厌此次活动，不想继续下去

10. 打卡

**用户任务：** 如果在活动进行前，发起者设置了系统推荐的这一活动过程中的打卡任务，则在活动过程中各成员可以相互合作、共同探索，完成小任务

**用户感受：** 
11. 分享

**用户任务：** 

**用户感受：** 

12. 反馈

**用户任务：** 

**用户感受：** 

13. 举报

**用户任务：** 

**用户感受：** 

#### iii.用户体验地图

### d)功能
#### i.网站功能及其目标
1. 需求

**功能：** 满足用户需求。
         
**目标：** 网站要能够满足用户产生的各种相关需求，使用户具有良好舒适的使用体验。
         
2. 账户    
         
**功能：** 注册阶段中，用户输入相关信息，系统经过校验确认无误后为用户注册账号并开辟个人空间。登陆阶段中，用户输入登陆所需的确认信息，待系统进行一定身份鉴定后允许用户以其身份访问站点并获取各种服务。
         
**目标：** 实现对账户统一有效的管理，确保用户身份唯一可用，维护数据库的安全新和完整性。在用户的登陆和注册过程中，给予用户即时、有效的反馈，同时考虑网站的视觉效果的呈现与流程的合理引导。
         
3. 个性化  
         
**功能：** 用户要求修改个人信息抑或是装扮个人空间，平台开启对应会话，并提供用户可用的修改信息的接口，待用户修改完毕并确认提交后，在后台保存用户的个性化数据，并将其在页面上呈现出来。当用户要求对个人评论、帖子进行管理时，平台仅提供可管理的相关数据和相应接口。
         
**目标：** 为用户提供的接口要考虑用户的接受度和可操作性。在保证良好的视觉效果的同时，应当使个性化流程易操作、可交互，使用户具有较好的修改体验。同时要合理限制用户的修改权限，用户只能修改仅与自身有关的数据。
         
4. 浏览    
         
**功能：** 平台将各种信息以一定的方式呈现在用户视野供用户获取信息，当用户进行页面的跳转时平台也要进行相应的信息更新，随着时间的推移平台信息应当发生相应变化。
         
**目标：** 实现信息的分类化、有序化和层次化。首先要根据信息本身的内容将其放在不同板块方便用户跳转，其次信息的排布要呈现一定的顺序，减轻用户浏览时的筛选负担，最后用户最关心，最符合用户需求的信息应当最先显示。
         
5. 邀约    
         
**功能：** 为用户提供发起邀约帖子的服务接口，提供模板协助用户完成邀约帖子的内容拟定，为用户提供与活动相适应的系列活动如打卡任务，将用户的邀约帖子发送到平台上进行展示，并向用户确认帖子已发起，之后随时向用户通知帖子的进展程度。
         
**目标：** 减轻用户在拟定邀约帖子内容时的思考负担，丰富活动内容，增加活动乐趣和吸引度，为用户吸引召唤具有参加活动条件和活动意愿的其他用户，使用户能了解自己邀约帖子的反馈情况。
         
6. 搜寻    
         
**功能：** 用户在搜索框输入自己想要的活动项目、时间等信息，系统为其展示最新的相关的邀约帖子。如果没有，系统为其提供发起帖子的建议，并根据用户搜索的关键词自动补充帖子的部分信息
         
**目标：** 帮助用户找到与自己想要参与的活动相关的帖子，如果没有就协助用户自己创建帖子
         
7. 评论    
         
**功能：** 用户可以在任何活动邀约帖子或者资讯帖子下面留下自己的想法、感受、问题
         
**目标：** 在活动邀约帖子下面评论，能让用户进一步对发起者的活动、计划进行了解，如果想法合拍，就可能相互组队；在资讯帖子下面评论，有利于激发用户的积极性，也能让其他对这条资讯感兴趣的人与此用户产生交集，制造相互交流乃至组队的机会
         
8. 应约    
         
**功能：** 用户点击“加入群组”按钮即可决定参加发起者的活动，准备参加活动，与其他成员交流
         
**目标：** 让用户能够与自己有好感的人一起、参与自己感兴趣的活动
         
9. 联系    
         
**功能：** 活动开始前后过程中，活动的各个成员可以在群组里保持联系
         
**目标：** 让用户们在不用添加联系方式的情况下，在活动中以匿名的方式相互联系，方便活动的开展
         
10. 打卡    
         
**功能：** 
         
**目标：** 
         
11. 分享    
         
**功能：** 
         
**目标：** 
         
12. 反馈    
         
**功能：** 
         
**目标：** 
         
13. 举报    
         
**功能：** 
         
**目标：** 

#### ii.网站功能图

# 四、技术实现方法
## 1.程序语言

## 2.设计软件

## 3.开发平台
