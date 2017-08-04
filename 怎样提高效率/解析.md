从上一章节中，我们得知我们现在已经得到了链接，下面我们就可以通过GET/POST方式发送请求，得到目标网站的回应.然后根据返回的资源格式的不同，分门别类的采取对应措施来解析取的数据.绝大多数都是业界主流的html格式还有就是前面章节里提到的JSON。

  
首先我们来说说html.HTML作为如今网页的基础，为互联网发展做出了巨大的贡献.一般我们用来解析HTML是通过DOM来解析的.

HTML DOM是HTML Document Object Model\(文档对象模型\)的缩写，HTML DOM则是专门适用于HTML/XHTML的文档对象模型。熟悉软件开发的人员可以将HTML DOM理解为网页的API。它将网页中的各个元素都看作一个个对象，从而使网页中的元素也可以被计算机语言获取或者编辑。 例如Javascript就可以利用HTML DOM动态地修改网页。而其他语言也都有类似的解析DOM包，比如golang的[goquery](https://github.com/PuerkitoBio/goquery),javascript的[cheerio](https://github.com/cheeriojs/cheerio),python的[BeautifulSou](https://www.crummy.com/software/BeautifulSoup/)L.

  
而网络世界除了HTML语言外，JSON也在为互联网的繁荣贡献自己的力量.JSON\(JavaScript Object Notation\)作为一种轻量级的数据交换格式.它基于 ECMAScript \(w3c制定的js规范\)的一个子集，采用完全独立于编程语言的文本格式来存储和表示数据.为前后端交互数据来达到动态网页的效果提供了一种易于人阅读和编写，同时也易于机器解析和生成的数据结构.

JSON结构很通俗易懂，在得知JSON结构后，可以很容易的从字符串里取出自己想要得到的数据.各种语言也提供了很多第三方的json解析包，比如[gjson](https://github.com/tidwall/gjson)\(golang\),[JSON-js](https://github.com/douglascrockford/JSON-js)\(Javascript\)等等.

