---
title: SignatureLine类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 640
url: /zh/python-net/aspose.cells.drawing/signatureline/
is_root: false
---
## SignatureLine类
代表签名行。



SignatureLine 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [SignatureLine()](/cells/zh/python-net/aspose.cells.drawing/signatureline/__init__/#) |构造 SignatureLine 的新实例|


### 特性
|属性|描述|
| :- | :- |
| [id](/cells/zh/python-net/aspose.cells.drawing/signatureline/id) |获取或设置此签名行的标识符。|
| [provider_id](/cells/zh/python-net/aspose.cells.drawing/signatureline/provider_id) |获取和设置签名提供者的id。|
| [signer](/cells/zh/python-net/aspose.cells.drawing/signatureline/signer) |获取和设置签名者。|
| [title](/cells/zh/python-net/aspose.cells.drawing/signatureline/title) |获取并设置歌手的称号。|
| [email](/cells/zh/python-net/aspose.cells.drawing/signatureline/email) |获取和设置歌手的电子邮件。|
| [is_line](/cells/zh/python-net/aspose.cells.drawing/signatureline/is_line) |指示它是否是签名行。|
| [allow_comments](/cells/zh/python-net/aspose.cells.drawing/signatureline/allow_comments) |指示是否可以附加评论。|
| [show_signed_date](/cells/zh/python-net/aspose.cells.drawing/signatureline/show_signed_date) |指示是否显示签名日期。|
| [instructions](/cells/zh/python-net/aspose.cells.drawing/signatureline/instructions) |获取和设置在签名时向用户显示的文本。|



### 例子

```python
from aspose.cells import Workbook
from aspose.cells.drawing import SignatureLine

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# Adding a picture
imgIndex = worksheet.pictures.add(1, 1, "sample.png")
pic = worksheet.pictures[imgIndex]
#  Create signature line object
s = SignatureLine()
s.signer = "Simon Zhao"
s.title = "Development Lead"
s.email = "Simon.Zhao@aspose.com"
#  Assign the signature line object to Picture.SignatureLine property
pic.signature_line = s
# do your business
# Save the excel file.
workbook.save("result.xlsx")

```

### 也可以看看
* 模块 [aspose.cells.drawing](..)
