DDD-Implement
=============
##Requirement One
公司A希望为员工成立各种俱乐部。

*    俱乐部的会长可以邀请会员
*    俱乐部的会员可以发起活动
*    会长审批活动。
*    俱乐部的会员可以参加活动
*    不同俱乐部的活动会有一些基本要求

##Requirement Two
这个需求以会话形式展开。
人物：客户（C），开发（D）

D：我们了解了您上次提出的需求，分析了下您的主要问题是如何组织一个俱乐部的活动。  
C：其实呢，作为一个会长头，我更关心俱乐部的预算。我最头疼的事情是每到季末，我们要出一份关于预算怎么花，举办了哪些活动的报表。  
D：那这个预算是一个什么概念呢？  
C : 俱乐部创建的时候，都会有一笔预算。这个预算用于俱乐部的活动，打个羽毛球啦什么的。  
D：那每次活动都会走这个预算？  
C：确实每次活动完了，都会报销一下。  
D：这个报销和我们的预算怎么发生关系的？  
C：就是发起活动的人，可以把预算减去活动的钱
D：谁都可以，跟公司财务有关系么？  
C：俱乐部的会员都可以。实际上会长会手动的填单子报销，现在这个阶段系统不用考虑到财务报销这个环节。    
D：好的。那提到了会员，我们想知道下会长怎么邀请会员和答复呢？必须是公司员工么？  
C：哦，肯定是公司的员工啊！一般我们通过发邮件的方式来邀请，如果确认加入就回封邮件。哎，这个我觉得很多网站发的邀请邮件里有个链接，一点这个链接就到它们网站上完成注册了。  
D：那会长怎么知道有哪些员工和他们的电邮？  
C：奥这个啊，公司有一个统一的员工联系方式记录。
D：那注册流程还有什么特殊的事情么？
C：没有了。哦对了，一个俱乐部的预算和会员数量有关，我们财务订了几个档，根据我们的会员数分配不同的预算。  
D：那这个预算怎么来修改呢，会长自己修改一下数额就好了？  
C：不是，这个得公司来审批的。就是当俱乐部的人数达到一定数量以后，会长会提出增加预算的申请，财务人员会来审批这个申请。  
D：财务人员来审批？那这个审批流程是在我们的俱乐部管理系统里么？  
C：是的。  
D：那就是说到现在为止，我们系统里会有三种用户。会长，会员和财务。财务是登陆到系统里，就可以审批预算申请了么？  
C：是的。  
D：财务人员还有其他的活动么？  
C：没有。  
D：那我们在一个俱乐部里组织活动是一个什么样的流程呢？  
C：就是会员可以发起一个活动，邀请其他会员参加  
D：这个可以发起活动的会员包括会长么  
C：包括。  
D：那我们通过什么方式邀请会员参加，和会员确认要参加呢？  
C：通过发Email吧，会员回复Link的形式。  
D：那活动的基本要求怎么提出呢，需要一些基本的填写模板和自动的审核流程么？  
C：哦这件事，没有这么复杂，写在活动的备注里，让会员看就可以了。  
D：那会长审批活动，主要是审批哪些内容呢？  
C：主要是活动的开销数额？  
D：就是活动要报销的？  
C：对，也不是所有的都需要审核。如果活动的预计花费大于剩余预算的一半，才需要会长审核。  
D：OK。
##Requirement Three
公司的职员通过单点登录系统获得访问公司内部不同网站的权利。
会员系统期初的时候会通过命令行的方式导入俱乐部信息到系统中
公司职员可以浏览所有的俱乐部以及俱乐部活动。