# Database数据库
## 一、 基本概念：
1. 数据：是指存储在某一种媒体上能够识别的物理符号。包括“数据内容”和“数据形式”两个方面
2. 数据处理：是指将数据转换成信息的过程。即从大量的数据中找出对人有用的数据的过程。
## 二、 计算机数据管理：
1. 利用计算机设备对数据进行分类、组织、编码、存储、检索和维护。
2. 发展过程：人工管理、文件管理、数据库系统、分布式数据库系统、面向对象的数据库系统。
## 三、 数据库系统
1. 数据库：（DB）是存储在计算机存储设备上，结构化的相关数据集合。它不仅包括描述事物的数据本身，还包括相关事物之间的联系。
   * 指按特定的组织形式将数据保存在存储介质上-特点:
     * 在数据库中，不仅包含数据本身，也包含数据之间的联系;
     * 数据通过一定的数据模型进行组织，保证有最小的冗余度，有层次、网状和关系模型;
     * 各个应用程序共享数据;
     * 对数据的各种操作，如定义、操纵等都由DBMS统一进行。
2. 数据库系统：(DBS)引进数据库技术后的计算机系统，实现有组织地、动态地存储大量相关数据，提供数据处理和和信息共享的便利手段。
3. 数据库管理系统：（DBMS）是位于用户与操作系统之间的一类通用的软件系统(对数据库进行管理的软件)，它由一组计算机程序组成。数据库管理系统能够对数据库进行有效的管理，这其中包括存储管理、安全性管理、完整性管理等，可以对数据库进行包括定义、查询、更新以及各种控制等操作。它是在数据库系统中对数据进行管理的系统软件，是数据库系统的核心组成部分，用户能够方便快捷地建立、维护、查询、存取和处理数据库中数据。例如,Microsoft Access 2010就是关系型桌面数据库管理系统。
   * 功能:
     * 定义:定义数据库的结构、数据完整性和其它的约束条件;
     * 操纵:实现数据插入、修改、删除和查询;
     * 控制:实现数安全控制、完整性控制以及多用户环境下的并发控制;
     * 维护:提供对数据的装载、转储和恢复，数据库的性能分析和监测;
     * 数据字典，存放数据库各级结构的描述。
4. 数据库应用系统：(DBAS) 是针对某一个实际应用管理对象而进行设计开发的面向用户的软件系统。它是建立在DBMS基础之上，具有较好的人机交互操作性和友好的用户界面。如学生管理系统、图书馆管理系统、民航售票系统等都是数据库应用系统。
5. 数据库用户
   * 终端用户具体使用和操作数据库应用系统,通过应用系统的用户界面使用数据库来完成其业务活动
   * 应用程序员以用户需求为基础、负责应用系统的开发设计编程，并进行调试和安装
   * 系统分析员负责应用系统的需求分析与规范说明,需要从总体上了解、设计整个系统, 确定系统的软硬件配置并参与数据库各级模式的概要设计
   * 数据库管理员 （DBA）负责整个数据库系统的建立、管理、维护以及所有使用系统人员的协调工作等。
## 四、 数据库系统的特点
1. 实现数据共享，减少数据冗余
2. 采用特定的数据模型
3. 具有较高的数据独立性
4. 有统一的数据控制功能
## 五、 数据库管理系统：是数据库系统的核心
1. 功能：数据定义、数据操作、数据库运行管理、数据组织、存储和管理、数据库建立和维护、数据通信接口
2. 组成：数据定义语言及翻译处理程序、数据操纵语言及其编译（或解释）程序、数据库运行控制程序、实用程序
## 六、数据库的分类
* 分布式数据库系统
  1. 数据库技术和计算机网络技术相结合产生:
     * 物理上独立，数据分布在网络的不同计算机
     * 逻辑上属于一个整体。
* 面向对象的数据库
  2. 将程序设计语言中对象的概念引用到数据库中:
     * 数据和操作方法作为对象统一管理;
     * 可以处理更为复杂的对象;
## 七、数据库系统的体系结构
* 三级模式
  1. 模式(逻辑模式或概念模式)是对数据库中的全部数据的逻辑结构和特征的描述，不涉及数据的物理存储。
  2. 外模式(用户模式或子模式)该模式面向用户，是数据库用户看到的局部数据结构和特征的描述，是数据的局部逻辑结构。
  3. 内模式(存储模式)描述数据的物理结构、在存储介质上的存储方法和存取策略。
* 二级映射(于三级模式之间的转换)
  1. 外模式/模式映射:定义外模式和概念模式之,间的对应性，这一-映射使得概念模式的改变不影响外模式和应用程序，从而达到了数据的逻辑独立性。
  2. 模式/内模式映射:定义概念模式和内模式之间的对应性，当存储结构改变即修改内模式时，只要相应改变模式/内模式映象，而模式尽量保存不变，从而达到了数据的物理独立性。
![alt](https://github.com/APF668899/Database/blob/master/REP01.png?raw=true)
## 八、数据库系统的位置
|数据库系统的位置||
|:---|:---|
|应用程序|用户|
|开发工具软件|数据库管理员|
|数据库管理系统|数据库管理员|
|操作系统|
|硬件|
   
