ghost太坑，并没有嵌套的二级导航，所以折腾了几天自己弄了一个出来。
此主题是复制于ghost的官方casper主题，实现以下几个功能：
1、用jquery实现显示二级导航；
2、文章目录导航
3、搜索

一、主导航：
导入此主题后，修改SECONDARY NAVIGATION的label为以下方式
<一级导航标签>|<二级导航标签>
![image](https://github.com/zhousmq/ghosttheme/blob/main/readme/menu.png)

二、文章目录导航
导入此主题后，进入后台， 在Code Injection修改Site Header和Site Footer里面加上以下两段代码
![image](https://github.com/zhousmq/ghosttheme/blob/main/readme/code.png)

三、搜索
导入此主题后，进入后台，进入Integrations，最下面的CUSTOM INTEGRATIONS，添加一个自定义integration，(name设置为content)，添加完成后会有一个key（示例：39.......d59be），复制此key；
再到在Code Injection修改Site Footer里面加上以下搜索必须用到的js代码
![image](https://github.com/zhousmq/ghosttheme/blob/main/readme/search.png)

最后：
感谢万能的google
感谢ghost博主https://huhao.ai/ghost-casper-theme-commets-search-toc-highlight/
