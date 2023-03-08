---
title: set_footer方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 180
url: /zh/python-net/aspose.cells/pagesetup/set_footer/
is_root: false
---
##  set_footer(section, footer_script) {#int-str}
设置格式化 Excel 文件页脚的脚本。



```python
def set_footer(self, section, footer_script):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| section | int |0：左部分，1：中部分，2：右部分。|
| footer_script | str |页脚格式脚本。|
### 评论

脚本命令：

|命令|描述|
| :- | :- |
|&P|当前页码|
|&N|页数|
|&D|当前日期|
|&T|当前时间|
| ＆A|工作表名称|
| ＆F|没有路径的文件名|
| &"<FontName>"|字体名称，例如：&"宋体"|
| &"<FontName>, <FontStyle>"|字体名称和字体样式，例如：&"Arial,Bold"|
| &<FontSize>|字体大小。如果此命令后跟要在标题中打印的普通数字，它将与字体高度用空格字符分隔。|
| &K<RRGGBB>|字体颜色，例如（红色）：&KFF0000|
| ＆G|图片脚本|

例如：“&Arial,Bold&8Footer Note”


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [PageSetup](/cells/zh/python-net/aspose.cells/pagesetup)
