---
title: "枚举 OpenDocumentFormatVersionType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Ods.OpenDocumentFormatVersionType 枚举。Open Document Format 版本类型"
type: docs
url: /zh/net/aspose.cells.ods/opendocumentformatversiontype/
---
## OpenDocumentFormatVersionType enumeration

Open Document Format 版本类型。

```csharp
public enum OpenDocumentFormatVersionType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| None | `0` | 无严格。 |
| Odf11 | `1` | ODF 版本 1.1 |
| Odf12 | `2` | ODF 版本 1.2 |
| Odf13 | `3` | ODF 版本 1.3 |
| Odf14 | `4` | ODF 版本 1.4 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OpenDocumentFormatVersionTypeDemo
    {
        public static void OpenDocumentFormatVersionTypeExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 向工作表添加一些数据
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);

            // 创建 OdsSaveOptions 并设置 ODF 版本
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;

            // 使用指定的 ODF 版本将工作簿保存为 ODS 格式
            workbook.Save("OpenDocumentFormatVersionTypeExample.ods", saveOptions);

            Console.WriteLine("Workbook saved successfully with ODF version 1.2.");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


