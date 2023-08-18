# 外接知识库

知识库相当于机器人的外接大脑，给它超出ChatGPT、超出公开数据集的知识储备，能在特定领域拥有更强的能力。

用例：接入项目文档/产品文档来回答用户/合作方的ad hoc questions；接入学术文献成为该领域专家；接入某人博客、推文成为数字生命；……

目前支持的链接方式有:

* [Gitbook](https://www.gitbook.com/)
* [Docusaurus](https://docusaurus.io/)
* 普通网页

更多输入形式的支持（离线文档、文本、Notion）正在开发中。

## 如何开始使用知识库功能?

在机器人的编辑页面中, 点击'知识库', 即可开始为机器人外接知识库

![](<../../.gitbook/assets/image (23).png>)

## 如何让知识库更好地为机器人服务?

1. 尽量使用文本类的网页. 对于大段文本类的网页, Myshell知识库能够很好地进行解析与回复. 相反地, 如果是一些非结构类(比如纯表格, 带有很多图片和复杂格式)的网页, Myshell知识库会有点力不从心.
2. 导入的多个知识库是同一个类型的. 对于导入了多个知识库的机器人, 不同的知识库如果是同一种类型或者内容相近的, 可以发挥出更好的效果. 比如我们如果想要制作一个某个动漫人物的机器人, 并且通过知识库补全动漫相关的人物讯息和世界观, 那么如果需要导入多个知识库的话, 最好都是跟这个动漫相关的.

## 小贴士

#### Gitbook使用小贴士

Gitbook是投喂bot知识库的重要方式

网址：[https://app.gitbook.com/](https://app.gitbook.com/)&#x20;

内容组织形式可参考MyShell的官方文档[https://docs.myshell.ai/](https://docs.myshell.ai/)&#x20;

编辑页面:

【注意】将文本内容写入/粘贴/导入到gitbook页面中，页面中所附的文件、在线链接、图像音频等多媒体内容均无法读取。&#x20;

【注意】需要在Team Space中创建页面，在Private Space中创建页面在分享时会有权限问题。

【内容写入】分模块式的内容组织，像写notion文档/飞书文档/Google文档一样使用。自己组织内容时一般只会“commands”中的以下几个block。

【页面分级】如内容层级较多，可在左侧页面编辑栏开设不同页面。

【页面分享】点击编辑页面右上方的“Share”，打开“Publish to the web”的按键，然后点击左下方“Copy published link”，将该链接粘贴到app.myshell.ai机器人创建过程中要求提供gitbook链接的地方。

【内容更新】页面公开发布后，页面右上方的“Share”会转为"Edit"，如需编辑内容可以点击"Edit"进入编辑页面。编辑好后点击“Merge”，更新的内容会自动同步。

#### 5分钟给你崽填充新鲜热乎知识库 | 轻松抓取网络材料

1. **抓取网页，获得材料**：HTTrack Website Copier 只需要输入你想抓取的网页，这个小工具就会把这个网页及其子网页的全部内容都下载下来 工具下载链接：[https://www.httrack.com/page/2/](https://www.httrack.com/page/2/)&#x20;
2. **导入gitbook，批量投喂** 小工具抓取到的内容都是html格式，你需要把所有需要的html复制到一个文件夹，压缩为.zip文件 然后就可以使用gitbook的批量import功能啦！ (已编辑)

**Q: 有时候HTTrack爬取的内容不全怎么办？** 如，一个主站有若干子链接，每个子链接都是需要的内容。而当内容过多的时候，HTTTrack无法提取所有子链接内容。&#x20;

**A: 这时候需要先获取所有需要获取的子链链接**，然后再使用HHTrack逐个爬取&#x20;

**方法1:** 使用Sitemap功能获得该网站全部链接，筛选出你需要的界面 如何创建Sitemap，使用插件或在线网站：[https://www.xml-sitemaps.com/](https://www.xml-sitemaps.com/) 筛选过程视工作量可手动或自动，若内容过多，可以请bot帮你写个小脚本解决（图1）&#x20;

**方法2:** 使用浏览器插件Easy Web Data Scraper获取所有链接 需要简单设置爬取方式、加载方式，即可自动爬取 链接：[https://chrome.google.com/webstore/detail/easy-web-data-scraper/mndkmbnkepbhdlkhlofdfcmgflbjggnl](https://chrome.google.com/webstore/detail/easy-web-data-scraper/mndkmbnkepbhdlkhlofdfcmgflbjggnl)&#x20;

**方法3:** 对于内容不多的爬取，使用插件Link Gopher 如果你需要爬取的链接可以在一个页面内加载完，使用这个插件可以最简单地提取 链接：[https://sites.google.com/site/linkgopher/](https://sites.google.com/site/linkgopher/)\
