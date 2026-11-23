---
title: "枚举 SensitivityLabelMarkType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Metas.SensitivityLabelMarkType 枚举。表示应应用于文件的内容标记类型"
type: docs
url: /zh/net/aspose.cells.metas/sensitivitylabelmarktype/
---
## SensitivityLabelMarkType enumeration

表示应应用于文件的内容标记类型。

```csharp
[Flags]
public enum SensitivityLabelMarkType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| None | `0` | 无 |
| Header | `1` | 页眉 |
| Footer | `2` | 页脚 |
| Watermark | `4` | 水印 |
| Encryption | `8` | 加密 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class MetasClassSensitivityLabelMarkTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 演示 SensitivityLabelMarkType 枚举值
            SensitivityLabelMarkType markType = SensitivityLabelMarkType.Watermark;

            // 根据类型应用不同的敏感度标签标记
            switch (markType)
            {
                case SensitivityLabelMarkType.None:
                    Console.WriteLine("No sensitivity label applied");
                    break;
                case SensitivityLabelMarkType.Header:
                    worksheet.PageSetup.SetHeader(0, "CONFIDENTIAL");
                    break;
                case SensitivityLabelMarkType.Footer:
                    worksheet.PageSetup.SetFooter(0, "INTERNAL USE ONLY");
                    break;
                case SensitivityLabelMarkType.Watermark:
                    worksheet.PageSetup.SetHeader(0, "&KFF0000&DRAFT");
                    break;
                case SensitivityLabelMarkType.Encryption:
                    workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, 128);
                    break;
            }

            // 保存已应用敏感度标签的工作簿
            workbook.Save("SensitivityLabelMarkTypeDemo.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


