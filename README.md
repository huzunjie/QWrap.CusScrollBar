QWrap.CusScrollBar
==================

基于QWrap的自定义滚动条插件(不提供UI方案,可自定义UI,按参数设置绑定)

使用示例:
<pre>
 
     <div class="source" style="font-family: '[object HTMLOptionElement]', Consolas, 'Lucida Console', 'Courier New'; color: rgb(0, 0, 0); "><span style="color: rgb(0, 0, 128); font-weight: bold; ">&lt;div</span> <span style="color: rgb(255, 0, 0); ">class=</span><span style="color: rgb(0, 0, 255); ">&quot;main&quot;</span><span style="color: rgb(0, 0, 128); font-weight: bold; ">&gt;</span><br> &nbsp; &nbsp;........... 内容们........<br><span style="color: rgb(0, 0, 128); font-weight: bold; ">&lt;/div&gt;</span><br><span style="color: rgb(0, 0, 128); font-weight: bold; ">&lt;div</span> <span style="color: rgb(255, 0, 0); ">class=</span><span style="color: rgb(0, 0, 255); ">&quot;scroll-wrap&quot;</span> <span style="color: rgb(255, 0, 0); ">style=</span><span style="color: rgb(0, 0, 255); ">&quot;position:relative;width:5px; height:500px;&quot;</span> <span style="color: rgb(255, 0, 0); ">title=</span><span style="color: rgb(0, 0, 255); ">&quot;滚动条容器&quot;</span><span style="color: rgb(0, 0, 128); font-weight: bold; ">&gt;</span><br> &nbsp;<span style="color: rgb(0, 0, 128); font-weight: bold; ">&lt;div</span> <span style="color: rgb(255, 0, 0); ">class=</span><span style="color: rgb(0, 0, 255); ">&quot;scroll-slider&quot;</span> <span style="color: rgb(255, 0, 0); ">style=</span><span style="color: rgb(0, 0, 255); ">&quot;position:absolute;top:0;width:5px; height:50px; background-color:#ddd;&quot;</span> <span style="color: rgb(255, 0, 0); ">title=</span><span style="color: rgb(0, 0, 255); ">&quot;滚动条滑块&quot;</span><span style="color: rgb(0, 0, 128); font-weight: bold; ">&gt;</span><br> &nbsp;<span style="color: rgb(0, 0, 128); font-weight: bold; ">&lt;/div&gt;</span> &nbsp;<br><span style="color: rgb(0, 0, 128); font-weight: bold; ">&lt;/div&gt;</span><br><br><span style="color: rgb(0, 0, 128); font-weight: bold; ">&lt;script&gt;</span><br><span style="color: rgb(0, 0, 128); font-weight: bold; ">var</span> <span style="color: rgb(0, 0, 0); ">myScroll</span> <span style="color: rgb(0, 0, 0); ">=</span> <span style="color: rgb(0, 0, 128); font-weight: bold; ">new</span> <span style="color: rgb(0, 0, 0); ">CusScrollBar</span><span style="color: rgb(0, 0, 0); ">({</span><span style="color: rgb(0, 0, 0); ">scrollDir</span><span style="color: rgb(0, 0, 0); ">:</span><span style="color: rgb(0, 0, 255); ">&quot;y&quot;</span><span style="color: rgb(0, 0, 0); ">,</span><span style="color: rgb(0, 0, 0); ">contSelector</span><span style="color: rgb(0, 0, 0); ">:</span><span style="color: rgb(0, 0, 255); ">&quot;.main&quot;</span><span style="color: rgb(0, 0, 0); ">,</span><span style="color: rgb(0, 0, 0); ">scrollBarSelector</span><span style="color: rgb(0, 0, 0); ">:</span><span style="color: rgb(0, 0, 255); ">&quot;.scroll-wrap&quot;</span><span style="color: rgb(0, 0, 0); ">,</span><span style="color: rgb(0, 0, 0); ">sliderSelector</span><span style="color: rgb(0, 0, 0); ">:</span><span style="color: rgb(0, 0, 255); ">&quot;.scroll-slider&quot;</span><span style="color: rgb(0, 0, 0); ">});</span><br><span style="color: rgb(0, 0, 128); font-weight: bold; ">&lt;/script&gt;</span><br></div>

  

</pre>

参数说明:
<pre>
        {
            scrollDir:"y",           //滚动条方向          [必填项,x||y,默认y]
            contSelector:"",         //内容容器元素选择器  [必填项]
            scrollBarSelector:"",    //滚动条模拟元素选择器[非必填项,如果为空则自动取sliderSelector的父容器]
            sliderSelector:"", //滚动条滑块          [必填项]
            addBtnSelector:"",       //滚动条坐标增加按钮(横向的向右,纵向的向下按钮)
            subBtnSelector:"",  //滚动条坐标减少按钮(横向的向左,纵向的向上按钮)
            btnClkStepSize:60,      //增加减少按钮按下时自动滚动的幅度
            addStepSize:30,          //滚动条坐标增加按钮每点击一次增加的幅度
            subtractStepSize:30,     //滚动条坐标减少按钮每点击一次减少的幅度
            sliderMinHeight:10,      //滑块最小高度
            sliderAlwaysShow:false,  //滑块是否保持显示(false则按照内容是否超出容器高度自动控制)
            scrollAnimTime:80,       //单次scrollToX 或 scrollToY所使用的动画时长
            scrollStepTime:10,       //scrollToX 或 scrollToY动画每帧时长
            scrollAnimAwait:false,   //滚动条动画是否等待上一帧完毕才执行交互响应
            wheelStepSize:80,       //滚轮控制滚动时,每次滚动触发的位移距离
            autoInitUiEvent:true    //是否自动初始化UI事件绑定
        }
<pre>
