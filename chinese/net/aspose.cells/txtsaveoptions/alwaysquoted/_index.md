---
title: "TxtSaveOptions.AlwaysQuoted"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TxtSaveOptions 属性。指示是否始终为每个字段添加 '\\\"'。如果为 true，则所有值都会加引号；如果为 false，则仅在需要时加引号，例如当值包含特殊字符如 '\\n' 或分隔符字符时。默认值为 false"
type: docs
url: /zh/net/aspose.cells/txtsaveoptions/alwaysquoted/
---
## TxtSaveOptions.AlwaysQuoted property

指示是否始终为每个字段添加 '\"'。如果为 true，则所有值都会加引号；如果为 false，则仅在需要时加引号（例如，当值包含特殊字符如 '\"'、'\n' 或分隔符字符时）。默认值为 false。

```csharp
[Obsolete("Use QuoteType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AlwaysQuoted { get; set; }
```

### 备注

注意：此成员现已过时。请改用 QuoteType 属性。此属性将在自 2012 年 8 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyAlwaysQuotedDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200.50);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(899.99);

            // 创建 TxtSaveOptions 并将 AlwaysQuoted 设置为 true
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Separator = ',',
                AlwaysQuoted = true,
                QuoteType = TxtValueQuoteType.Always
            };

            // 保存时在所有值周围加引号
            workbook.Save("AlwaysQuoted_True.txt", saveOptions);

            // 更改为 false 并再次保存
            saveOptions.AlwaysQuoted = false;
            workbook.Save("AlwaysQuoted_False.txt", saveOptions);

            Console.WriteLine("Files saved with different AlwaysQuoted settings.");
        }
    }
}
```

### 另请参见

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


