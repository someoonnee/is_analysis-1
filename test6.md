﻿<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

## 实验6（期末考核） 基于GitHub的实验管理平台的分析与设计 | [返回](./README.md)

- 本课程是考查课程，期末考查内容是完善老师的<b>基于GitHub的实验管理平台</b>
- 课程平台是：http://202.115.86.207/ ，是同学们真实的成绩。
- 老师现在的实验管理平台只是一个最简单的平台，即<b>三单</b>（单学期，单课程，单评分项），
只考虑了一个学期，一门课程，没有考虑多个学期，多门课程，多评分项实验。现在的实验管理平台中一共有5个实验，每个实验只有一个评分项（0-100分）和对应的文字性的评价。
  对于期末课程设计等较大型的实验不能按评分项精确评价学生的实验情况，实验成绩的主观性较强。
- 需要同学们完善的地方是将**三单改为三多**（多学期，多课程，多评分项）：    
    - 一个老师可以上多门课，每个老师只能维护老师自己的课程及成绩。
    - 一人同学可以上多门课，每个同学只能查询同学自己的课程的实验成绩。
    - 必须考虑选课了，老师和同学都可以选多门课程，但必须是老师先选，学生后选。
    - 原实验为<b>单评分项</b>实验，<b>要求改为多评分项实验</b>，即每个实验的实验成绩细分为多个评分项，每个评分项对应各自的评分标准。
      老师在批改实验的时候，对每个评分项进行评分并输入对应的文字评价，系统自动计算出所有评分项的成绩之和为该实验的总成绩。
    - 考虑到有多个学期，每个学期都有不同的实验。
    - 系统设计在界面上和操作上应该方便老师查询和评阅学生的实验成绩，应该方便学生查询实验成绩。 
    - 思考：如果要将这个实验评分平台推广到全国使用，应该考虑多学校，又该怎么设计呢？
    
- 期末考核要求
    - 需要同学们完成系统分析与设计，并写成<B>一组详细设计文档</B>，以README.md作为设计文档的先导文件。
    所有文档不需要写成Word或者Excel，就以Markdown形式加超链接形式互相链接即可，最后发布到你的GitHUB上。
    - 对于PlantUML图，文档中只需要直接显示图片，不需要直接出现PlantUML源码，但需要提供链接，链接中能显示PlantUML源码。
    - 文档提交目录：期末考核的所有文档均在目录test6中。
    - 文档编写参照实验2至实验5的要求。
    - 将以上文档再组合成一个Word类型的最终文档[design.docx](./test6/design.docx)，该文件和README.md放在一个目录中。在design.docx中也应该包括目录与模块之间跳转。**design.docx必须打印出来上交给老师**。
- 注意事项
    - 原则上，用例图只有一个，类图只有一个
    - 原则上，顺序图应该是每个用例一个，用于描述用例的业务流程
    - 活动图用于描述一个不是显而易见的算法或者顺序图不方便描述的业务流程。数量不限。
    - 用例规约表编写见表第7章Page147表7.5，不要以截图方式，要以表格方式编写。
    - 需要同学们写出所有用例，所有界面。越详细越好。
    - 抄袭的同学期末考试成绩为0分！！
    
- 本实验采用多评分项方式评分，评分项及评分标准是（总分100分）：
    
    |评分项|评分标准|分数|
    |:-------|:----------------------|:------|
    |文档整体|文档内容详实、规范，美观大方|20|
    |用例图及规约|用例图完整，准确，能够完全体现需求|10|
    |顺序图与活动图|顺序图能够完全描述用例的设计思路和业务流程，活动图能够描述部分算法的流程。|10|
    |类图|类图能够完整，准确反映业务的需数据的组织结构|10|
    |数据库|数据库表的设计来自于类图，合理|10|
    |界面设计|界面设计美观，清晰，合理，能够完全反映用例图的设计思路|10|
    |API接口设计|为每个界面设计合理的API接口，以便进行前后端分离开发|15|
    |内容一致性|用例图，类图、数据库、界面相互印证，相互依赖，环环相扣|15|

<b>实验提交</b>

- 实验提交到自己的gitHub的is_analysis/test6目录中，主要文件名是：README.md，再附上一些图片文件。
- 你的gitHub中的is_analysis/test6目录中可能有以下文件：

``` filelist
README.md
pic1.png
...
```

- 你的实验内容提交成功后，可以直接访问https://github.com/<b>zhang</b>/is_analysis/tree/master/test6
查看你编写的实验文档。其中zhang是你的gitHub用户名。

- 期末考核（含打印的纸质报告）**最终提交时间：2019年5月6日（第11周星期一）**。过时扣分。

<b>参考</b>

- AXURE界面设计工具参见： https://www.axure.com/
- RESTful API 设计指南参见：http://www.ruanyifeng.com/blog/2014/05/restful_api.html
- RESTful API 设计样例参见：http://os.opensns.cn/book/index/read/id/5.html
- 获得北京天气预报的API: https://www.sojson.com/open/api/weather/json.shtml?city=北京
- Markdown格式参考：https://www.jianshu.com/p/b03a8d7b1719
- 老师的教学资源：https://github.com/zwdbox/is_analysis
- 老师做的<b>基于GitHub的实验管理平台</b>参考：https://github.com/zwdbox/is_analysis/tree/master/test6