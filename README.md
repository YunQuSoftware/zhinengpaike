# 基于java、SQLServer 毕业设计 智能排课系统的设计与实现
第一章 系统概述
1．1  智能排课系统概述
智能排课系统是一个教育单位不可缺少的部分,它的内容对于学校的决策者和管理者来说都至关重要,所以智能排课系统应该能够为用户提供充足的信息和快捷的查询手段。但一直以来人们使用传统人工的方式管理文件排课，这种管理方式存在着许多缺点,如:效率低、保密性差,另外时间一长,将产生大量的文件和数据,这对于查找、更新和维护都带来了不少的困难。随着科学技术的不断提高,计算机科学日渐成熟,其强大的功能已为人们深刻认识,它已进入人类社会的各个领域并发挥着越来越重要的作用。作为计算机应用的一部分,使用计算机对排课信息进行管理,具有着手工管理所无法比拟的优点。例如：检索迅速、查找方便、可靠性高、存储量大、保密性好、寿命长、成本低等。这些优点能够极大地提高智能排课的效率,也是企业的科学化、正规化管理,与世界接轨的重要条件。

1．2智能排课系统的目的和意义
终上所述，开发这样一套智能排课软件成为很有必要的事情。我们所开发的这智能排课软件归纳起来，好处大约有以下几点：
1． 可以存储历届的排课，安全、高效；
2． 只需一到二名排课录入员即可操作系统，节省大量人力；
3． 可以按照录入人员的输入来自动生成课程表，并尽量减少冲突等情况发生。 
排课系统的设计分析根据实际情况，我们使用原型法（Rapid Prototyping）即以少量代价快速地构造一个可执行的软件系统模型。使用户和开发人员可以较快地确定需求，然后采用循环进化的开发方式，对系统模型作连续的精化，将系统需具备的性质逐渐增加上去，直到所有的性质全部满足。此时模块也发展成为最终产品了。
第二章 开发平台的技术
2.1 JAVA简介
Java是目前最常用的计算机编程语言，也是主要的网络开发语言之一。Java具有面向对象、分布式和多线程等先进高级计算机语言的特点，同时它还因可移植、安全性能高和网络移动性等逐渐成为一种行业标准。对于初次接触计算机编程语言的人来说，Java语言简单易学，不需要长时间的培训就可以编写出适合现在企业或个人需要的程序。
Java的特点：
(1). 平台无关性
平台无关性是指Java能运行于不同的平台。Java引进虚拟机 原理，并运行于虚拟机，实现不同平台的Java接口之间。使 用Java编写的程序能在世界范围内共享。Java的数据类型与 机器无关，Java虚拟机（Java Virtual Machine）是建立在 硬件和操作系统之上，实现Java二进制代码的解释执行功能， 提供于不同平台的接口的。
(2). 安全性 
Java的编程类似C++,学习过C++的读者将很快掌握Java的精 髓。Java舍弃了C++的指针对存储器地址的直接操作，程序 运行时，内存由操作系统分配，这样可以避免病毒通过指 针侵入系统。Java对程序提供了安全管理器，防止程序的 非法访问。
(3). 面向对象
Java 吸取了C++面向对象的概念，将数据封装于类中,利用类的优点，实现了程序的简洁性和便于维护性。类的封装性、继承性等有关对象的特性，使程序代码只需一次编译，然后通过上述特性反复利用。程序员只需把主要精力用在类和接口的设计和应用上。Java提供了众多的一般对象的类，通过继承即可使用父类的方法。在Java中，类的继承关系是单一的非多重的，一个子类只有一个父类，子类的父类又有一个父类。Java提供的 Object类及其子类的继承关系如同一棵倒立的树形，根类为Object 类，Object 类功能强大，经常会使用到它及其 它派生的子类。
(4). 分布式
Java建立在扩展TCP/IP网络平台上。库函数提供了用HTTP和FTP协议传送和接受信息的方法。这使得程序员使用网络上的文件和使用本机文件一样容易。
(5). 键壮性
Java致力于检查程序在编译和运行时的错误。类型检查帮助检查出许多开发早期出现的错误。Java自己操纵内存减少了内存出错的可能性。Java还实现了真数组，避免了覆盖数据的可能。这些功能特征大大提高了开发Java应用程序的周期。Java提供：Null指针检测、数组边界检测、异常出口、Byte code校验。
2.2 JSP简介
JSP是Sun公司推出的新一代网站开发语言，Sun公司借助自己在Java上的不凡造诣，将Java从Java应用程序和Java Applet之外，又有新的硕果，就是JSP，Java Server Page。JSP可以在Serverlet和JavaBean的支持下，完成功能强大的站点程序。使用JSP技术，Web页面开发人员可以使用HTML或者XML标识来设计和格式化最终页面。使用JSP标识或者小脚本来产生页面上的动态内容。产生内容的逻辑被封装在标识和JavaBeans群组件中，并且捆绑在小脚本中，所有的脚本在服务器端执行。如果核心逻辑被封装在标识和Beans中，那么其它人，如Web管理人员和页面设计者，能够编辑和使用JSP页面，而不影响内容的产生。在服务器端，JSP引擎解释JSP标识，产生所请求的内容（例如，通过存取JavaBeans群组件，使用JDBC技术存取数据库），并且将结果以HTML（或者XML）页面的形式发送回浏览器。这有助于作者保护自己的代码，而又保证任何基于HTML的Web浏览器的完全可用性。
绝大多数JSP页面依赖于可重用且跨平台的组件（如：JavaBeans或者Enterprise JavaBeans）来执行应用程序所要求的更为复杂的处理。开发人员能够共享和交换执行普通操作的组件，或者使得这些组件为更多的使用者或者用户团体所使用。基于组件的方法加速了总体开发过程，并且使得各种群组织在他们现有的技能和优化结果的开发努力中得到平衡。
Web页面开发人员不会都是熟悉脚本语言的程序设计人员。Java Server Page技术封装了许多功能，这些功能是在易用的、与JSP相关的XML标识中进行动态内容产生所需要的。标准的JSP标识能够存取和实例化 JavaBeans组件，设定或者检索群组件属性，下载Applet，以及执行用其它方法更难于编码和耗时的功能。
通过开发定制化标识库，JSP技术是可以扩展的。今后，第三方开发人员和其它人员可以为常用功能建立自己的标识库。这使得Web页面开发人员能够使用熟悉的工具和如同标识一样的执行特定功能的构件来工作。
JSP技术很容易整合到多种应用体系结构中，以利用现存的工具和技巧，并且扩展到能够支持企业级的分布式应用。作为采用Java技术家族的一部分，以及Java 2EE的一个成员，JSP技术能够支持高度复杂的基于Web的应用。
由于JSP页面的内置脚本语言是基于Java程序设计语言的，而且所有的JSP页面都被编译成为Java Servlet，JSP页面就具有Java技术的所有好处，包括健壮的存储管理和安全性。
作为Java平台的一部分，JSP拥有Java程序设计语言“一次编写，各处执行”的特点。随着越来越多的供货商将JSP支持加入到他们的产品中，您可以使用自己所选择的服务器和工具，修改工具或服务器并不影响目前的应用。
2.3 Tomcat的介绍
Tomcat是Apache Jakarta软件组织的一个子项目，Tomcat是一个JSP/Servlet容器，它是在SUN公司的JSWDK（Java Server Web Development Kit）基础上发展起来的一个JSP和Servlet规范的标准实现，使用Tomcat可以体验JSP和Servlet的最新规范。经过多年的发展，Tomcat不仅是JSP和Servlet规范的标准实现，而且具备了很多商业Java Servlet容器的特性，并被一些企业用于商业用途。粗略地可以将servlet容器分为如下几类:
	独立的servlet容器
内置有web服务器的一部分。指当使用基于Java的web服务器的情形,例如servlet容器是JavaWebServer的一个部分。独立的servlet容器是Tomcat的默认模式。大多数的web服务器并非基于Java，因此，我们可以得出如下两种容器的模式。
	进程内的servlet容器
servlet容器作为web服务器的插件和Java容器的实现。Web服务器插件在内部地址空间打开一个JVM(java virtual machine)使Java容器得以在内部运行.如有某个需要调用servlet的请求，插件将取得对此请求的控制并将他传递(使用JNI)给Java容器。进程内容器对于多线程，单进程的服务器非常合适并且提供很好的运行速度，但伸缩性有所不足。
	进程外的servlet容器
servlet容器运行于web服务器之外的地址空间且作为web服务器的插件和Java容器的实现的结合.web服务器插件和Java容器 JVM使用IPC机制(通常是TCP/IP)进行通讯.当一个调用servlet的请求到达时,插件将取得对此请求的控制并将其传递(使用IPC等)给Java容器,进程外容器的反应时间或进程外容器引擎不如进程内容器,但进程外容器引擎在许多其他可比的范围内更好(伸缩性,稳定性等)。
Tomcat既可作为独立的容器(主要是用于开发与调试)又可作为对现有服务器的附加(当前支持Apache,IIS和Netscape服务器).即任何时候配置Tomcat你都必须决定如何应用他,如选择第二或第三种模式,你还需要安装一个web服务器接口。~

基于Java、MySQL的毕业设计，智能排课系统 专业定制计算机专业毕业设计，QQ：1184131126，公众号：计算机专业毕业设计（ITJSZXG）
