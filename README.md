1,针对bootstrap 开发.
2,无刷新自动提交插件.
3,依赖jQuery name : ajaxxy ajaxxy.t(调用翻译事件) ajaxxy.submit(自动提交事件)
使用方法:引入插件,from表单下的 buttom(type=submit) 会自动提交.

使用方法:
<script src="ajaxxy.js" type="text/javascript"></script>
例如有以下表单
<form id="form1"></form>
ajaxxy("#form1").set()//设置该表单的提交属性

ajaxxy.set()//设置全局表单的提交属性

ajaxxy.set(option,[help]) option该表单的提交属性,help(boolean),是否打印设置帮助.

-------ajaxxy opgion 设置帮助-------

 (1) functionName:回调函数 -> 以window()形式调用

 (2) callback:回调执行函数

 (3) prefixback:前置函数,在没有提交时执行.

 (4) unique:必须校验的input,即input不能为空值

 (5) abandon:是否跳过所有的表单验证,优先级不如 unique

 (6) alert:是否显示返回的警告信息

 (7) alertStyle:显示的警告信息的样式 warning | success | dismissable | danger

 (8) alertTo:警告内容的显示元素 #xxx | .xxx 字符串,由$ 获取

 (9) alertLocation:显示在元素的位置 before | after | self(内部)

 (10) alertMax:警告最多显示多少条

 (11) debug:是否开启调试

 (12) callbackScroll:执行完回调函数后scroll是否运动

 (13) scrollTop:scroll运动到那个px

 (14) confirm:提交时是否二次确认

 (15) confirmText:提交时是否二次确认文字

 (16) jsonp:是否跨域请求

 (17) jsoncallback:跨域回调函数名

 (18) ajaxErrorCallback:ajax错误回调函数

 (19) timeout:Ajax超时时间

