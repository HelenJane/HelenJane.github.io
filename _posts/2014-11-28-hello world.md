---
layout:default
title:hello world
date: 2014-11-26 16:35:40
---
<h2>{{page.title}}</h2>
<p>my first page </p>

<p>{{page.date|date: "%b %-d, %Y"}}</p>

<body>
<div id="disqus_thread"></div>
<script type="text/javascript">
/* * * CONFIGURATION VARIABLES: EDIT BEFORE PASTING INTO YOUR WEBPAGE * * */
var disqus_shortname = 'hellohelenjane'; // required: replace example with your forum shortname
/* * * DON'T EDIT BELOW THIS LINE * * */
(function() {
var dsq = document.createElement('script'); dsq.type = 'text/javascript'; dsq.async = true;
dsq.src = '//' + disqus_shortname + '.disqus.com/embed.js';
(document.getElementsByTagName('head')[0] || document.getElementsByTagName('body')[0]).appendChild(dsq);
})();
$('#disqus_container .comment').on('click',function(){
$(this).html('加载中...');
var disqus_shortname = 'hellohelenjane';
var that = this;
BYB.includeScript('http://' + disqus_shortname + '.disqus.com/embed.js',function(){$(that).remove()}); //这是一个加载js的函数
});
</script>
</body>

