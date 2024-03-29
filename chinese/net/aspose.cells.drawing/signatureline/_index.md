---
title: SignatureLine
second_title: Aspose.Cells for .NET API 参考
description: 代表签名行
type: docs
weight: 2770
url: /zh/net/aspose.cells.drawing/signatureline/
---
## SignatureLine class

代表签名行。

```csharp
public class SignatureLine
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [SignatureLine](signatureline)() | 默认构造函数。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [AllowComments](../../aspose.cells.drawing/signatureline/allowcomments) { get; set; } | 表示是否可以附加评论。 |
| [Email](../../aspose.cells.drawing/signatureline/email) { get; set; } | 获取和设置歌手的邮箱。 |
| [Id](../../aspose.cells.drawing/signatureline/id) { get; set; } | 获取或设置此签名行的标识符。 |
| [Instructions](../../aspose.cells.drawing/signatureline/instructions) { get; set; } | 获取并设置在签名时向用户显示的文本。 |
| [IsLine](../../aspose.cells.drawing/signatureline/isline) { get; set; } | 表示是否为签名行。 |
| [ProviderId](../../aspose.cells.drawing/signatureline/providerid) { get; set; } | 获取并设置签名提供者的id。 |
| [ShowSignedDate](../../aspose.cells.drawing/signatureline/showsigneddate) { get; set; } | 表示是否显示签名日期。 |
| [Signer](../../aspose.cells.drawing/signatureline/signer) { get; set; } | 获取和设置签名者。 |
| [Title](../../aspose.cells.drawing/signatureline/title) { get; set; } | 获取并设置歌手的标题。 |

### 例子

```csharp

[C#]

//实例化一个工作簿对象
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];

//添加图片
int imgIndex = worksheet.Pictures.Add(1, 1, "sample.png");
Picture pic = worksheet.Pictures[imgIndex];
// 创建签名线对象
SignatureLine s = new SignatureLine();
s.Signer = "Simon Zhao";
s.Title = "Development Lead";
s.Email = "Simon.Zhao@aspose.com";
// 将签名线对象分配给 Picture.SignatureLine 属性
pic.SignatureLine = s;

//做你的事

//保存excel文件。
workbook.Save("result.xlsx");
```

### 也可以看看

* 命名空间 [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
