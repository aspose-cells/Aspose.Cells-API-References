---
title: "枚举 SignatureType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Drawing.SignatureType 枚举。指定签名类型"
type: docs
url: /zh/net/aspose.cells.drawing/signaturetype/
---
## SignatureType enumeration

指定签名类型。

```csharp
public enum SignatureType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Default | `0` | 默认值，对应的 ProviderId 值固定为 {0000000000-0000-0000-0000-0000000000}。 |
| Stamp | `1` | 对应的 ProviderId 值通常为 {000CD6A4-0000-0000-C000-000000000046}。 |
| Custom | `3` | 对应的 ProviderId 值通常需要用户设置。它应当从随提供程序附带的文档中获取。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassSignatureTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加不同类型的签名行
            Picture stampPicture = worksheet.Shapes.AddSignatureLine(3, 1, new SignatureLine());
            stampPicture.SignatureLine.SignatureLineType = SignatureType.Stamp;

            Picture customPicture = worksheet.Shapes.AddSignatureLine(8, 1, new SignatureLine());
            customPicture.SignatureLine.SignatureLineType = SignatureType.Custom;
            customPicture.SignatureLine.ProviderId = new Guid("12345678-ABCD-4321-5678-9876543210AB");

            // 保存带有签名配置的工作簿
            workbook.Save("SignatureTypeDemo.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


