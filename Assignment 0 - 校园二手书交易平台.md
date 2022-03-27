# Assignment 0 - 校园二手书交易平台

## 1. 团队信息
- 队名: HuangDuSAD
- 成员: 
  - 2052526 白俊豪
  - 2053025 何庐坤
  - 2053285 罗斌江
  - 2052540 王艳天


## 2. 项目背景
​	书籍在大学生的日常学习生活中扮演着不可或缺的角色，无论是课本、工具还是小说等文学作品，既增加了学生的专业知识，又丰富了他们的精神世界。 但是，目前有以下几个现象致使书籍无法得到更加有效地利用：

- 教科书在课程结束后遭遇闲置和废弃等结局

- 文学作品在阅读以后就被束之高阁

- 很多专业书籍的价格令人却步

  而另一方面，

- 某些书店的二手书折旧率太低，但售价偏高，赚取高额差价。同学们的出手和入手意愿不高。

- 某些书籍资料发行较少，在学校以外难以找到。

- 拥有闲置书的人和有购买需求的人之间缺乏桥梁。

​	为了让书籍得到更加充分有效的利用，并且让同学经济快捷地获取自己想要的书籍，建立一个开放包容的以二手书交易为主的多元化共享平台是有必要的。


## 3. 主要目标（项目内容）
1. 全面应用面向对象，结合‎在系统分析设计‎课程中学到的内容，为系统制定合理的规划，强化系统设计与分析的能力。
2. 为书籍的交易提供便利，为买书和卖书的人之间提供桥梁。
3. 提供书籍捐赠服务，暂存用户捐赠的书籍到图书馆或爱心公益亭，避免书籍的不合理浪费。
4. 与校方合作，根据各个课程老师的要求，为校园用户提供购书推荐。


## 4. 主要内容和特点

### 内容

​	通过网页构建一个卖家和买家交流的平台，为双方提供以下服务：

1. 买家浏览书籍
2. 买家寻求特定的书籍，并且可以发布求书请求
2. 根据学生的课程为他们推荐书籍
3. 卖家将闲置的书籍出售
4. 爱心人士捐赠书籍

### 特点

​	功能特点：

- 不需要的图书妥善处理
- 针对专业年级推荐书籍和卖家

​	技术特点：

- 采用UML设计，为开发团队提供统一的设计建模。
- 使用面向对象的思想，具有重用性、灵活性、可拓展性

​	应用层面特点：

- 针对校园用户，用户规模小，服务更精确




## 5. 目标用户和可用性目标
### 目标用户

1. Students who have a lot of unused textbooks at the end of the semester and have no way to dispose of them
2. Students who have spent too much money to buy textbooks at the beginning of the semester
3. Students who need a used book but can't find it in the market
4. 希望捐赠书籍的学生：通过平台与学校图书馆和爱心公益亭联系，将书籍妥善保管。

### Usability goals

1. Compared with traditional bookstores, the process of earning price difference is reduced, so that students can get books at a lower price.
2. Compared to online book buying, on-campus book trading reduces the delivery process and is more convenient and fast
3. The market is concentrated on campus, and the book inventory is more abundant and targeted


## 6. 现有同类产品分析

Compared with Confucius Used Books, Used Books Street, etc., this platform has the following advantages
1. The platform is more accurate in terms of groups and landing areas (students and schools), and the corresponding books are more abundant
2. The transaction scope is concentrated in the school, which saves the seller shipping cost and the buyer can get the purchased books on the same day.
3. Linkage with the school academic system, providing guidance for students' book purchases

## 7. 解决方案的新颖性

- 平台向所有同学开放，在已知同学相关信息的情况下可以根据培养方案向其推荐书籍
- 为买卖双方提供交流平台，买家可以发布求购信息，买卖双方借助搜索引擎可以迅速取得联系
- 与图书馆、爱心公益亭合作，将由同学捐赠的书籍录入数据库，妥善存放，免费提供给需要的同学。

## 8. 可能遇到的挑战

- 许多学生的私人数据存储在用户管理系统中，应合理规划不同角色的数据查看权限，并增加相应的安全控制条件，以达到保护个人隐私的目的。
- 用户在系统中注册时应进行严格的验证和调查，对用户书籍的交易也应当进行适当限制，以免有心人士借用该平台不正当牟利。
- 领取存放在图书馆、爱心公益亭的书籍应经过手续并有一定限制，做到物尽其用。
- 确定系统边界并采用适当的技术进行项目开发。
- 为了自给自足地长期运营，如何更好地与商业广告沟通是未来Web开发将面临的问题。

## 9. 相关技术

1. 建模：UML
2. 数据库：Mysql
3. 前端：Vue，Bootstrap
4. 服务端：Spring，SpringMVC，MyBatis
5. 架构：B/S

## 10. 项目相关资源

### 10.1 参考项目地址

1. [基于ssm的校园二手交易平台](https://github.com/wsk1103/Used-Trading-Platform)
2. [二手书交易系统](https://github.com/DaDaDouDouer/atschool)

### 10.2 相关资料

1. [“石大众阅享书网”二手书交易平台的分析与实现](https://www.cnki.com.cn/Article/CJFDTOTAL-KXZG201714069.htm)
2. [Spring Framework Reference](https://docs.spring.io/spring-framework/docs/current/reference/html/core.html#spring-core)