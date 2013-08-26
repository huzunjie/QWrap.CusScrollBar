QWrap.CusScrollBar
==================

基于QWrap的自定义滚动条插件(不提供UI方案,可自定义UI,按参数设置绑定)


使用示例:
<pre>
 
     <div class="source" style="font-family: '[object HTMLOptionElement]', Consolas, 'Lucida Console', 'Courier New'; color: rgb(0, 0, 0); "><span style="color: rgb(0, 0, 128); font-weight: bold; ">&lt;div</span> <span style="color: rgb(255, 0, 0); ">class=</span><span style="color: rgb(0, 0, 255); ">&quot;main&quot;</span><span style="color: rgb(0, 0, 128); font-weight: bold; ">&gt;</span><br> &nbsp; &nbsp;........... 内容们........<br><span style="color: rgb(0, 0, 128); font-weight: bold; ">&lt;/div&gt;</span><br><span style="color: rgb(0, 0, 128); font-weight: bold; ">&lt;div</span> <span style="color: rgb(255, 0, 0); ">class=</span><span style="color: rgb(0, 0, 255); ">&quot;scroll-wrap&quot;</span> <span style="color: rgb(255, 0, 0); ">style=</span><span style="color: rgb(0, 0, 255); ">&quot;position:relative;width:5px; height:500px;&quot;</span> <span style="color: rgb(255, 0, 0); ">title=</span><span style="color: rgb(0, 0, 255); ">&quot;滚动条容器&quot;</span><span style="color: rgb(0, 0, 128); font-weight: bold; ">&gt;</span><br> &nbsp;<span style="color: rgb(0, 0, 128); font-weight: bold; ">&lt;div</span> <span style="color: rgb(255, 0, 0); ">class=</span><span style="color: rgb(0, 0, 255); ">&quot;scroll-slider&quot;</span> <span style="color: rgb(255, 0, 0); ">style=</span><span style="color: rgb(0, 0, 255); ">&quot;position:absolute;top:0;width:5px; height:50px; background-color:#ddd;&quot;</span> <span style="color: rgb(255, 0, 0); ">title=</span><span style="color: rgb(0, 0, 255); ">&quot;滚动条滑块&quot;</span><span style="color: rgb(0, 0, 128); font-weight: bold; ">&gt;</span><br> &nbsp;<span style="color: rgb(0, 0, 128); font-weight: bold; ">&lt;/div&gt;</span> &nbsp;<br><span style="color: rgb(0, 0, 128); font-weight: bold; ">&lt;/div&gt;</span><br><br><span style="color: rgb(0, 0, 128); font-weight: bold; ">&lt;script&gt;</span><br><span style="color: rgb(0, 0, 128); font-weight: bold; ">var</span> <span style="color: rgb(0, 0, 0); ">myScroll</span> <span style="color: rgb(0, 0, 0); ">=</span> <span style="color: rgb(0, 0, 128); font-weight: bold; ">new</span> <span style="color: rgb(0, 0, 0); ">CusScrollBar</span><span style="color: rgb(0, 0, 0); ">({</span><span style="color: rgb(0, 0, 0); ">scrollDir</span><span style="color: rgb(0, 0, 0); ">:</span><span style="color: rgb(0, 0, 255); ">&quot;y&quot;</span><span style="color: rgb(0, 0, 0); ">,</span><span style="color: rgb(0, 0, 0); ">contSelector</span><span style="color: rgb(0, 0, 0); ">:</span><span style="color: rgb(0, 0, 255); ">&quot;.main&quot;</span><span style="color: rgb(0, 0, 0); ">,</span><span style="color: rgb(0, 0, 0); ">scrollBarSelector</span><span style="color: rgb(0, 0, 0); ">:</span><span style="color: rgb(0, 0, 255); ">&quot;.scroll-wrap&quot;</span><span style="color: rgb(0, 0, 0); ">,</span><span style="color: rgb(0, 0, 0); ">sliderSelector</span><span style="color: rgb(0, 0, 0); ">:</span><span style="color: rgb(0, 0, 255); ">&quot;.scroll-slider&quot;</span><span style="color: rgb(0, 0, 0); ">});</span><br><span style="color: rgb(0, 0, 128); font-weight: bold; ">&lt;/script&gt;</span><br></div>

  

</pre>

