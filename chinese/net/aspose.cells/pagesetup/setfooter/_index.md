---
title: SetFooter
second_title: Aspose.Cells for .NET API 参考
description: 设置格式化 Excel 文件页脚的脚本
type: docs
weight: 600
url: /zh/net/aspose.cells/pagesetup/setfooter/
---
## PageSetup.SetFooter method

设置格式化 Excel 文件页脚的脚本。

```csharp
public void SetFooter(int section, string footerScript)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| section | Int32 | 0：左侧部分，1：中间部分，2：右侧部分。 |
| footerScript | String | 页脚格式脚本。 |

### 评论

脚本命令：

**命令**

**描述**

&amp;P

当前页码

&amp;N

页数

&amp;D

当前的日期

&amp;T

当前时间

＆一个

工作表名称

＆F

没有路径的文件名

&amp;"&lt;字体名称&gt;"

字体名称，例如：&amp;"Arial"

&amp;"&lt;字体名称&gt;, &lt;字体样式&gt;"

字体名称和字体样式，例如：&amp;"Arial,Bold"

&amp;&lt;字体大小&gt;

字体大小。如果此命令后跟要打印在页眉中的纯数字，它将与字体高度用空格字符分隔。

&amp;K&lt;RRGGBB&gt;

字体颜色，例如（RED）：&amp;KFF0000

＆G

图像脚本

例如：“&amp;Arial,Bold&amp;8Footer Note”

### 也可以看看

* class [PageSetup](../../pagesetup)
* 命名空间 [Aspose.Cells](../../pagesetup)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
