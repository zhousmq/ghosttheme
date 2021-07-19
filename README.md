ghost太坑，并没有嵌套的二级导航，所以折腾了几天自己弄了一个出来。
此主题是复制于ghost的官方casper主题，用jquery实现显示二级导航，并加上了文章目录导航

一、主导航：
导入此主题后，修改SECONDARY NAVIGATION的label为以下方式
<一级导航标签>|<二级导航标签>

二、文章目录导航
导入此主题后，进入后台， 在Code Injection修改Site Header和Site Footer里面加上以下两段代码
<!--在Header中加载样式-->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/tocbot/4.11.1/tocbot.css">

<!--在Footer中加载js并初始化-->
<script src="https://cdnjs.cloudflare.com/ajax/libs/tocbot/4.11.1/tocbot.min.js"></script>
<script>
    tocbot.init({
        tocSelector: '.toc',
        contentSelector: '.post-content',
        headingSelector: 'h1, h2, h3',
    });
</script>
