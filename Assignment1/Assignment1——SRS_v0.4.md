# Assignment1——SRS

<center><font size=5 color=#008b8b>Content</font></center> 

[toc]

<div STYLE="page-break-after: always;"></div>
## 0.版本记录

| 版本号     | 说明         | 日期 |
| --------- | ----------- | ---|
| v0.1      | 初版需求 |    |

## 1.引言

在本节中，您将大致了解本文档中涉及的几乎所有内容，包括系统的简要说明、本文档的用途以及其他一些杂项内容。

### 1.1 编写目的



### 1.2 项目背景

书籍在大学生的日常学习生活中扮演着不可或缺的角色，无论是课本、工具还是小说等文学作品，既增加了学生的专业知识，又丰富了他们的精神世界。 但是，目前有以下几个现象致使书籍无法得到更加有效地利用：

- 教科书在课程结束后遭遇闲置和废弃等结局

- 文学作品在阅读以后就被束之高阁

- 很多专业书籍的价格令人却步

  而另一方面，

- 某些书店的二手书折旧率太低，但售价偏高，赚取高额差价。同学们的出手和入手意愿不高。

- 某些书籍资料发行较少，在学校以外难以找到。

- 拥有闲置书的人和有购买需求的人之间缺乏桥梁。

 为了让书籍得到更加充分有效的利用，并且让同学经济快捷地获取自己想要的书籍，建立一个开放包容的以二手书交易为主的多元化共享平台是有必要的。

### 1.3 读者对象和阅读建议

本 SRS 文件适用于参与该系统的人员。 只想对这款产品有个大致印象的读者引言部分已经足够。 而对于系统的特性、功能或依赖关系等更详细的信息，建议阅读第 2 部分（介绍）。

至于用例建模，在第三部分(Specific Requirement)中有专门的描述，在这里你也可以一窥系统的接口。其次，第 4 部分（补充规格）包括有关系统的一些附加信息。最后，第6部分展示了我们

### 1.4 术语表

| Terms                           | Definition                                                   |
| ------------------------------- | ------------------------------------------------------------ |
| **platform**                    | 由一组子系统和技术形成的软硬件设施。通过一些接口和使用模式提供了一组一致的功能，任何由它所支持的应用都可以使用这些功能而不必关心其实现细节。 |
| **user**                        | 具有访问计算机系统中的特定程序及数据权力的个人或组织。       |
| **log-in**                      | 用户输入用户名和密码或身份凭证，由系统验证身份，以确定是否允许进入系统的过程。 |
| **registration**                | 为一个实体登记一个名称。使感兴趣的用户可通过该名称访问这个实体。 |
| **query**                       | 为了在数据库中寻找某一特定文件、网站、记录或一系列记录，由搜索引擎或数据库送出的消息。 |
| **browsing**                    | 在网络中快速或粗略地阅读文档内容。通常是在导航期间进行。     |
| **personalized recommendation** | 根据用户的兴趣特点推荐其感兴趣的对象的活动。                 |
| **feedback**                    | 系统输出端的信息流（或包括物质流）回流到输入端的过程。反馈可从系统的输出端直接连接到输入端，也可经由系统的其他要素而传到输入端。 |
| **information distribution**    | 及时向项目各利害关系者提供所需信息的过程。                   |

## 2.介绍

### 2.1 产品概览

该系统是一个网页应用，包括网页端和服务器。服务器通过数据库和预先设定的程序来处理用户的不同请求，更为详细的说明在用例建模部分会有介绍。

### 2.2 产品特性

- 作为网页应用，任何拥有浏览器和网络的设备都可以访问并使用。
- 本系统设计时考虑并采用了严格的访问限制。用户只能访问自身权限以内的数据，且只有在获得授权后才能更改。
- 同学们不需要的图书可以被妥善处理。
- 针对专业年级推荐书籍和卖家
- 针对校园用户，用户规模小，服务更精确

### 2.3 参与者

本系统有两种参与者，用户和管理员，他们都有不可替代的作用。

用户可以浏览其他用户发布的信息以及系统推荐给

管理员负责审核用户发布的信息、管理用户及其捐赠的书籍


### 2.4 设定与依赖
本系统的运行依赖于一定的前提和外部支持：

- 与爱心公益亭、图书馆合作，将用户捐赠但暂时无人认领的书籍存放在指定位置，并将信息上传至数据库，方便需要的用户查找并领取。
- 本系统不提供直接的交易平台和担保，有交易意向的同学通过网站建立联系，简单交流，约定线下交易。
- 

## 3.用例建模

### 3.1敏捷开发和需求分析

### 3.2用例图

插图，描述

#### 总览



#### 详细用例规约：

##### 登录系统









Rigister

| Use Case         | Register |
| ---------------- | -------- |
| ID               |          |
| Specification    |    Visitors register their own account and fill their own basic information;System give authorization according to the type of the account.      |
| Actors           |      users    |
| Pre-condition    |     Visitors enter the login webpage for the first time and click "sign in".     |
| Basic Path       | 1. Visitors enter the website.<br/>2. Visitors click "sign up".<br/>3. Visitors fill basic information:<br/>    3.1 Visitors fill cellphone number\email.<br/>    3.2 Visitors set username and password. <br/>4. Visitors click "send verification code" and fill the code from text or email .<br/>5. Visitors successfully create an user account. |
| Alternative Path | 1. Visitors exit the webpage during information filling<br/>    system will show notification:"Information filling incomplete,do you want to exit anyway?"<br/>2. Visitors have problem during creating the account:<br/>    2.1 Visitors input illegal cellphone number\email<br/>           system will show notification:"Sorry,illegal cellphone number\email\"<br/>    2.2 Visitors don't receive verification code<br/>           system will allow visitors to resend the verification code again after 60s countdown.<br/>    2.3 Visitors input wrong verification code<br/>            system will show notification:"Sorry,wrong verification code,please input again."<br/> |
| Post-condition   | Visitors get their personal account and authorization.       |

Login

| Use Case         | Login |
| ---------------- | ----- |
| ID               |       |
| Specification    |       |
| Actors           |       |
| Pre-condition    |       |
| Basic Path       |       |
| Alternative Path |       |
| Post-condition   |       |

##### 交易系统

购买书籍

| Use Case         | 购买书籍 |
| ---------------- | -------- |
| ID               |          |
| Specification    |    Users buy the books they need and choose a satisfactory transaction method      |
| Actors           |     Users     |
| Pre-condition    |    The user selects the book of his choice and clicks on the "Buy" button      |
| Basic Path       |     1. Users selects the book of his choice<br/>  2. Users clicks on the "Buy" button<br/>  3. Users selects the satisfactory transaction method<br/>  3.1. Users choose how to pick up the book: Home delivery (if optional) or pick up from the seller<br/>  3.2. Users choose the payment method: in person/through the platform<br/>  4. the user selectively refines the transaction information: transaction time/place<br/>  5. the user submits the transaction application<br/>  6. return transaction application results<br/>  6.1 If the transaction result is successful, the corresponding transaction will be generated under the user<br/>  6.2 If the transaction results in failure, return the reasons for failure (incomplete information, etc.) |
| Alternative Path |     1. Visitors exit the webpage during information filling system will show notification: "Information filling incomplete,do you want to exit anyway?"<br/>2. If you choose to pay immediately, but do not pay after submitting the application, the transaction will fail and the reason will be returned<br/>3. If the time taken to complete the transaction request process exceeds the preset value, the transaction will fail and the system will show notification: "Transaction request has timed out"     |
| Post-condition   |       The user completes a transaction request   |

信息发布

| Use Case         | 信息发布 |
| ---------------- | -------- |
| ID               |          |
| Specification    |   Enables users to post requests, sales and donations of books       |
| Actors           |    User      |
| Pre-condition    |     the operator has a personal account      |
| Basic Path       |     1. Users click on the "Publish Information" button<br/>2. The user selects the type of information that needs to be posted: Wanted / Sold / Donated<br/>3. The user completes the corresponding information form<br/>4. User submits the information form to be published<br/>5. The background will review the information released<br/>6.return information release results<br/>6.1 If the information release is successful, Generate and publish the corresponding purchase/sale/donation information to the platform<br/>6.2 If the information release results in failure, return the reasons for failure (incomplete information, etc.)      |
| Alternative Path |      1. Visitors exit the webpage during information filling system will show notification: "Information filling incomplete,do you want to exit anyway?"<br/>2. If there are any omissions when submitting the information sheet, the submission will fail and the relevant prompt will be returned<br/>3. If the time taken to complete the process exceeds the preset value, the transaction will fail and the system will show notification: "Transaction reques    |
| Post-condition   |     Generate and publish the corresponding purchase/sale/donation information to the platform     |

Information Review

| Use Case         | Information Review |
| ---------------- | ----- |
| ID               |       |
| Specification    |    The administrator conducts a second review of postings whose content is deemed problematic by the system   |
| Actors           |    administer   |
| Pre-condition    |    The system passes a problematic release message to the administrator   |
| Basic Path       |   1. The administrator opens the release information passed by the system<br/>2. The administrator verifies the release information according to the questions raised by the system<br/>3. The administrator determines whether there is a problem with the release information<br/>3.1 If not, the system will release the information to the platform<br/>3.2 If there is, the information will be rejected and the reason will be sent to the publisher    |
| Alternative Path |    If the verification message is not processed within 24 hours, a message will be sent: "You have a message waiting for verification, please process it as soon as possible"    |
| Post-condition   |   The administrator ultimately decides whether the posting is normal or not, and decides whether to post on the platform    |

浏览及搜索商品

| Use Case         | 浏览及搜索商品 |
| ---------------- | -------------- |
| ID               |                |
| Specification    |       Users browse or search through the various types of information that have been published to find the books they need         |
| Actors           |      Users        |
| Pre-condition    |     None           |
| Basic Path       |       1. The user enters keywords in the search input box<br/>2. The user selects the tag information for the search (author, related fields...) <br/>3. The user clicks the "Search" button<br/>4. The platform returns books that match the corresponding search criteria         |
| Alternative Path |       If no book information is found that meets the criteria, return "Sorry, no information was found that meets the criteria, you can try to post a request"         |
| Post-condition   |        Users have access to detailed product information        |

交易反馈

| Use Case         | 交易反馈 |
| ---------------- | -------- |
| ID               |          |
| Specification    |    Allow clients to provide feedback to the platform on any problems or suggestions they encounter in their transactions     |
| Actors           |     Users      |
| Pre-condition    |     The user has completed or is in the process of completing a transaction     |
| Basic Path       |      1. Users click on the "Transaction Feedback" button<br/>2. Users fill out the transaction feedback information form<br/>3. The user submits the transaction feedback information form<br/>4. Users choose the degree of urgency of feedback    |
| Alternative Path |     1. Visitors exit the webpage during information filling system will show notification: "Information filling incomplete,do you want to exit anyway?"<br/>2. If the key information submitted in the information form is incomplete, the submission will fail and return relevant prompts     |
| Post-condition   |     Administrators can process feedback submitted     |

##### 图书管理系统

query books

| Use Case | query books |
| -------- | ----------- |
| ID       |             |
| 简要说明 |             |

##### 用户资料管理系统

修改个人资料

| Use Case | 修改个人资料 |
| -------- | ------------ |
| ID       |              |
| 简要说明 |       Users can improve and modify their personal information, such as grade, major, etc., so that the system can recommend relevant products for them based on their personal information.       |

### 3.3活动图

### 3.3.1注册

### 3.3.2登录

### 3.3.3购书

### 3.3.4信息发布

### 3.3.5审核信息

## 4.补充规格

### 4.1 补充规格说明

本文档旨在阐释二手书交易平台的需求和要求。在上面列出的用例建模无法颇为细致地说明软件的要求，因此在下面补充了软件的必需规格。

### 4.2 性能

软件的性能必须得到保证，这关乎用户的体验。

- 该系统并发度应该大于100
- 该系统单次请求响应时间需在0.5s之内
- 该系统同时荷载用户要求：游客>10000,用户大于5000

### 4.3 可靠性

本系统应具有可靠性，具体表现在：

- 在网络畅通并且用户数小于5000的情况下，一年内出问题的时间必须小于90min。在软件中不能有阻断性Bug

- 用户需求可变更：用户可以进行交易反馈，提出他们的问题并由管理员进行处理，进而快速反应进行处理。如果出现问题，反应时间不能大于1天。
- 用户需求需要得到精准的理解，系统应具有完整的需求定义
- 具有健壮性
- 对特殊情况和错误处理需要全面考虑

### 4.4 安全性

用户来源和发布的内容的安全性：

- 用户的注册需填写个人信息并审核
- 用户的登录需要用户名和密码相吻合
- 用户上架的内容需要管理员审核

用户安全得到保障：

- 用户可以凭借密保信息找回密码
- 用户可以随时修改个人资料

数据安全：

- 数据安全等级分级，敏感信息加密

- 数据的服务器储存在安全的位置，仅有获得权限的人可以访问

### 4.5 维护性

- 易于理解：建模设计结构化，建模描述充分，建模语言统一

- 便于修改：模块之间关系清晰明了，结构良好。低耦合，高内聚。
- 可移植性：把因环境变化而必须修改的程序局限在少数程序模块中，从而降低修改难度

- 可回退：每半小时，自动储存备份，可以回到上一个版本。
- 快速反应：当发生阻断错误时，应该在90min之内反应

### 4.6 可用性

- 用户界面友好，易于操作

 

## 5.SWOT分析矩阵

SWOT分析法是基于内外部环境和竞争条件下的态势分析，将与研究对象密切相关的各种主要内部优势、劣势和外部的机会和威胁等，通过调查列举出来，并依照矩阵形式排列，然后用系统分析的思想，把各种因素相互匹配起来加以分析，从中得出一系列相应的带有一定决策性的结论。

此处应有图

## 6.参考文献

[1]杨洋,刘全. 软件系统分析与体系结构设计[M].南京东南大学出版社:, 201710.207.

这本书主要内容包括软件工程概述、结构化分析和设计方法、面向对象的分析和设计方法以及软件体系结构设计。其中的3-7章中以UML为建模语言，给出了用例建模的完整例子，并给出了分析设计的方法。

[2]冀振燕. UML系统分析与设计教程[M].人民邮电出版社:, 201408.277.

这本书介绍了基础UML语言知识以及UML在系统分析与设计中的应用。其中对于如何使用UML语言进行了深入浅出的阐释。另外，在面向对象为基础的软件设计与分析方面，也给出了具体的例子。

[3]吕冠艳,李奋华.基于UML的信息系统需求分析模型[J].微型机与应用,2010,29(20):8-10+15.DOI:10.19358/j.issn.1674-7720.2010.20.003.
[4]屈喜龙.UML及面向对象的分析与设计的研究[J].计算机应用研究,2005(09):74-76.
[5]陈娟. 基于UML的面向对象的系统分析与设计[D].武汉理工大学,2005.
[6]孔军,孙怡宁,蒋敏,毕宝庆.基于UML的系统需求分析[J].计算机工程与应用,2003(15):217-219.
[7]王瑞金,段会川,Martin Gogolla.统一建模语言UML及其建模实例[J].计算机应用研究,2002(08):80-84.
[8]黄贤英.UML建模过程及在需求分析中的应用[J].计算机工程,2001(11):184-186.

## 7.成员贡献