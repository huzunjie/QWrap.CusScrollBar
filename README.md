QWrap.CusScrollBar
==================

基于QWrap的自定义滚动条插件(不提供UI方案,可自定义UI,按参数设置绑定)


使用示例:
<div class="main">
    ........... 内容们........
</div>
<div class="scroll-wrap" style="position:relative;width:5px; height:500px;" title="滚动条容器">
  <div class="scroll-slider" style="position:absolute;top:0;width:5px; height:50px; background-color:#ddd;" title="滚动条滑块">
  </div>  
</div>

<script>
var myScroll = new CusScrollBar({scrollDir:"y",contSelector:".main",scrollBarSelector:".scroll-wrap",scrollSliderSelector:".scroll-slider"});
</script>

