
```
															⊂ヽ
															　 ＼＼ ∧＿∧
															　　 ＼( ˘ω˘ )　
															　　　 　⌒ヽ
															　　　/ 　 へ＼
															　　 /　　/　＼＼
															　　 ﾚ　ノ　　 ヽ_つ
															　　/　/
															　 /　/|
															　(　(ヽ
															　|　|、＼
															　| 丿 ＼ ⌒)
															　| |　　) /
															`ノ )　 Lﾉ
															(_／

```
# AIO维护指南1

>写在前言：此文档主要针对AIO2012版的维护讲解,08版和09版对应的QQ版本已经封版，在这里就不在阐述；

### 前台文件:

>***Html***：发布系统—>`腾讯网迷你版`—>内容管理—>页面管理—>站点根目录

* AIO_html文件（测试）：mini_site_t.htm;
* AIO_html文件（正式版）：mini_site_index.htm;
* AIO_html文件（灰度版）：mini_site_gray.htm;
* SSI动态合并 ：SSItoPage.htm;
* 代理准备 ：proxy_ready.htm;

>***CSS***：发布系统—>`腾讯网迷你版`—>内容管理—>页面管理—>样式存储区

* AIO样式（测试版）☆☆：style_lib/mini_style_t.htm;
* AIO样式（灰度版）：style_lib/mini_style_gray.htm;
* AIO样式（正式版）：style_lib/mini_style_index.htm;

### 后台模板：
>发布系统—>`后台管理`—>模板管理—>模板列表

>***注***：上述路径基于已经登陆腾讯网迷你版的情况;

* 模板是基于XSLT和XML实现;
* 模板ID是提供给cms可视化的标识;
* 模板url是提供给SSItoPage.htm和mini_site_t.htm(mini_site_gray.htm/mini_site_index.htm)的标识;

### Cms可视化操作：

>发布系统—>`XX频道`—>内容管理—>AIO内容管理—>页卡编辑

* 左侧为可视化模板操作，用于编辑日常更新新闻;
* 右侧页卡模板选择(一般改版选择新模板的时候用);

### Example:

1. 后台管理新建频道模板;
2. 模板ID给到CMS同事，初始化处理，可视化操作可见;
3. 模板url添加到SSItoPage.htm和mini_site_t.htm;
4. 线上浏览：http://minisite2012.qq.com/test/AIO_Tool.htm;

###Build log:
* @author <a href="mailto:rex08@vip.qq.com">rexzhang</a>
* @version 1.0.0
* @date 2013-12-23

###UpDate log:

* @author <a href="mailto:rex08@vip.qq.com">rexzhang</a>
* @version 1.0.1
* @update 2013-12-24
* @info 修改XXX
