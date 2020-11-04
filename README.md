欢迎！这里是非官方的 REAPER API 中文文档。

## 这个文档和其他有什么区别？

中文 REAPER API 文档主要参考自：

- https://www.reaper.fm/sdk/reascript/reascripthelp.html
- https://mespotin.uber.space/Ultraschall/Reaper_Api_Documentation.html
- https://www.extremraym.com/cloud/reascript-doc

希望提供本地化的 REAPER API 说明，以及提供更详细的范例。更希望是有使用经验上的分享，如注意事项、使用范例等。

## 我可以怎么参与文档建设

你可以在这个填写表填写 API 信息：[REAPER API 填写表](https://docs.qq.com/form/page/DS1dRbkFSeXZGVXha)

操作非常简单，数据清洗和收集由我和脚本自动完成。每当有人提交一份新的表单，我会在后台收到并定期检查更新在文档网站上。

## 我想改进文档基础项目

本项目由 Sphinx 驱动，基于腾讯文档的问卷，与腾讯文档上 excel 表格做数据源。结合人工，采用项目根目录的 gen.ipynb 脚本来做数据清洗与格式化。

目前文档网站首页采用的 index.rst（在 source 里） 采用人工编辑，source 里面的其他所有内容基于上述数据源自动格式化。

你可以在此基础上作任意改动，并提交合并。
