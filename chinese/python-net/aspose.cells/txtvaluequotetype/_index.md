---
title: TxtValueQuoteType枚举
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 2610
url: /zh/python-net/aspose.cells/txtvaluequotetype/
is_root: false
---
## TxtValueQuoteType枚举
指定在文本格式文件中对值使用引号的类型。



TxtValueQuoteType 类型公开了以下成员：

### 领域
|场地|描述|
| :- | :- |
| NORMAL |所有包含特殊字符（如引号、分隔符）的值都将被引用。<br/>与 ms excel 导出文本文件的行为相同。|
| ALWAYS |所有值将始终被引用。|
| MINIMUM |仅在需要时引用值。例如，如果一个值包含引号但引号不在该值的开头，则该值将不会被引用。|
| NEVER |不会引用所有值。由于缺少所需的引号，因此可能无法正确回读此类型的导出文本文件。|



### 也可以看看
* 模块 [aspose.cells](..)
