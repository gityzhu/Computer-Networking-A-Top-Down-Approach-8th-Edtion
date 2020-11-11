# 计算机网络：自顶向下设计（第八版） 


自20年前出版第一版以来，这本书已在数百所大学和大学中采用，翻译成14种语言，并在全球范围内被数以百万计的学生和实践者使用。积极的回应使我们不知所措。

这本教科书是关于计算机网络的第一门课程。它已经在计算机科学和电气工程系，信息系统和信息学系，商学院以及其他地方（无论是本科生还是研究生）中使用。工业界的从业人员也应该对此感兴趣。在此处查找有关教科书的更多信息。

## 关于这本书

这本书适合谁？
这本教科书通常用于计算机网络的第一门课程。它已在计算机科学和电气工程系，信息系统和信息学系，商学院以及其他地方使用。就编程语言而言，这本书仅假设该学生具有C，C ++，Java或Python的经验（甚至在少数地方也是如此）。尽管这本书比许多其他计算机网络入门课本更为精确和分析性强，但它很少使用高中未教授的任何数学概念。我们努力避免使用任何高级演算，概率或随机过程概念（尽管我们为具有这种高级背景的学生提供了一些家庭作业问题）。因此，该书适合于本科课程和一年级研究生课程。这对工业从业者也应该是有用的。


自上而下的方法
计算机网络似乎非常复杂-毕竟，互联网在许多方面是人类有史以来最大的工程系统！网络涉及以复杂方式编织在一起的许多概念，协议和技术。为了应对这种范围和复杂性，许多计算机网络文本通常围绕网络体系结构的“层”进行组织。通过分层的组织，学生可以了解计算机网络的复杂性，他们可以了解体系结构某一部分中的独特概念和协议，同时可以看到各个部分如何组合在一起的全局视图。从教学的角度来看，我们的个人经验是，这种分层方法确实行之有效。但是，我们发现传统的教学方法是自下而上。那是，

我们的书在20年前通过以自上而下的方式处理网络（即，从应用程序层开始并逐步向下到物理层）来开拓了新的领域。我们从老师和学生那里收到的反馈都证实，这种自上而下的方法具有很多优势，并且在教学上确实有效。首先，它着重于应用程序层（网络中的“高增长领域”）。确实，计算机网络的许多最新革命（包括Web和媒体流）已在应用程序层发生。对应用层问题的早期强调与大多数其他文章中所采用的方法不同，后者仅对网络应用，其要求，应用层范例（例如，客户端-服务器和对等），和应用程序编程接口。其次，我们作为教师（以及使用过本书的许多教师）的经验是，在课程开始时教授网络应用程序是一种强大的激励工具。令学生兴奋的是，他们了解网络应用程序的工作原理，例如大多数学生每天使用的应用程序，例如电子邮件，流视频和Web。一旦学生了解了这些应用程序，就可以了解支持这些应用程序所需的网络服务。然后，学生可以依次检查可以在较低层中提供和实施此类服务的各种方式。因此，尽早覆盖应用程序将为本文的其余部分提供动力。我们作为教师的经验（以及许多使用过本文的教师的经验）一直认为，在课程开始时教网络应用程序是一种强大的激励工具。令学生兴奋的是，他们了解网络应用程序的工作原理，例如大多数学生每天使用的应用程序，例如电子邮件，流视频和Web。一旦学生了解了这些应用程序，就可以了解支持这些应用程序所需的网络服务。然后，学生可以依次检查可以在较低层中提供和实施此类服务的各种方式。因此，尽早覆盖应用程序将为本文的其余部分提供动力。我们作为教师的经验（以及许多使用过本文的教师的经验）一直认为，在课程开始时教网络应用程序是一种强大的激励工具。令学生兴奋的是，他们了解网络应用程序的工作原理，例如大多数学生每天使用的应用程序，例如电子邮件，流视频和Web。一旦学生了解了这些应用程序，就可以了解支持这些应用程序所需的网络服务。然后，学生可以依次检查可以在较低层中提供和实施此类服务的各种方式。因此，尽早覆盖应用程序将为本文的其余部分提供动力。令学生兴奋的是，他们了解网络应用程序的工作原理，例如大多数学生每天使用的应用程序，例如电子邮件，流视频和Web。一旦学生了解了这些应用程序，就可以了解支持这些应用程序所需的网络服务。然后，学生可以依次检查可以在较低层中提供和实施此类服务的各种方式。因此，尽早覆盖应用程序将为本文的其余部分提供动力。令学生兴奋的是，他们了解网络应用程序的工作原理，例如大多数学生每天使用的应用程序，例如电子邮件，流视频和Web。一旦学生了解了这些应用程序，就可以了解支持这些应用程序所需的网络服务。然后，学生可以依次检查可以在较低层中提供和实施此类服务的各种方式。因此，尽早覆盖应用程序将为本文的其余部分提供动力。研究可以在较低层中提供和实现这些服务的各种方式。因此，尽早覆盖应用程序将为本文的其余部分提供动力。研究可以在较低层中提供和实现这些服务的各种方式。因此，尽早覆盖应用程序将为本文的其余部分提供动力。

第三，自上而下的方法使教师可以在早期阶段引入网络应用程序开发。学生不仅了解流行的应用程序和协议如何工作，而且还了解创建自己的网络应用程序和应用程序级别协议的难易程度。通过自上而下的方法，学生可以更早地了解套接字编程，服务模型和协议的概念，这些重要概念会在随后的所有层中重新出现。通过提供Python套接字编程示例，我们突出了中心思想，而不会使学生难以理解复杂的代码。具有任何语言编程经验的读者都可以轻松掌握Python代码。


互联网焦点
尽管我们在第4版的书名中删除了“使Internet流行”一词，但这并不意味着我们就不再关注Internet。确实，此案无可厚非！相反，由于Internet变得如此普及，我们认为任何网络教科书都必须将重点放在Internet上，因此此短语在某种程度上是不必要的。我们将继续使用Internet的体系结构和协议作为研究基本计算机网络概念的主要手段。当然，我们还包括其他网络体系结构的概念和协议。但是，显然，Internet上有很多关注点，这一事实反映在我们围绕Internet的五层体系结构进行组织的书中：应用程序，传输，网络，链接和物理层。

聚焦互联网的另一个好处是，学生渴望了解互联网及其协议。他们知道互联网是一种革命性的颠覆性技术，可以看到它正在深刻改变着我们的世界。鉴于互联网的重要性，学生们自然对“幕后”感到好奇。因此，当使用互联网作为指导重点时，教师很容易激发学生对基本原理的兴趣。


教学网络原理
这本书的两个独特功能-自上而下的方法和对互联网的关注-出现在我们书的书名中。如果我们可以将第三个短语压缩到副标题中，它将包含“原则”一词。。现在，网络领域已经足够成熟，可以确定许多根本上重要的问题。例如，在传输层中，基本问题包括在不可靠的网络层上的可靠通信，连接建立/拆除和握手，拥塞和流量控制以及多路复用。从根本上来说，网络层的三个问题是确定两个路由器之间的“良好”路径，互连大量异构网络以及管理现代网络的复杂性。在链路层中，一个基本问题是共享多路访问通道。在网络安全性中，用于提供机密性，身份验证和消息完整性的技术都基于密码学基础。本文确定了基本的网络问题，并研究了解决这些问题的方法。学习这些原理的学生将获得长久的“保质期”知识—在当今的网络标准和协议过时很久之后，它们体现的原理将仍然重要且相关。我们认为，结合使用Internet吸引学生进入大门，然后强调基本问题和解决方案的方法，将使学生能够快速了解​​几乎任何网络技术。

# 本月要做的任务
- [ ] 更新PPT，实验资源
- [x] 完成部署工具的设置
- [ ] 增加思维导图
