---
title: "TxtLoadOptions.MaxRowCount"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TxtLoadOptions 属性。每个工作表要导入的最大行数"
type: docs
url: /zh/net/aspose.cells/txtloadoptions/maxrowcount/
---
## TxtLoadOptions.MaxRowCount property

每个工作表要导入的最大行数。

```csharp
public int MaxRowCount { get; set; }
```

### 备注

超过此限制的行将根据 [`ExtendToNextSheet`](../extendtonextsheet/) 被忽略或扩展到下一个工作表。此计数包括标题行（[`HeaderRowsCount`](../headerrowscount/)）。它的最大允许值是相应文件格式的行限制，例如对于 xlsx 文件为 1048576。如果未指定此属性或指定的值不是正数，则也将使用最大限制。

### 示例

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyMaxRowCountDemo
    {
        public static void Run()
        {
            // 创建示例 CSV 内容
            string content = "Header1,Header2,Header3\n" +
                            "Data1,Data2,Data3\n" +
                            "Data4,Data5,Data6\n" +
                            "Data7,Data8,Data9\n" +
                            "Data10,Data11,Data12\n" +
                            "Data13,Data14,Data15\n" +
                            "Data16,Data17,Data18";

            // 创建 TxtLoadOptions 并将 MaxRowCount 设置为 4
            TxtLoadOptions opts = new TxtLoadOptions
            {
                MaxRowCount = 4,  // Only load first 4 rows (including header)
                HeaderRowsCount = 1  // First row is header
            };

            // 将 CSV 加载到工作簿中
            using (MemoryStream ms = new MemoryStream(Encoding.UTF8.GetBytes(content)))
            {
                Workbook wb = new Workbook(ms, opts);

                // 验证仅加载了 4 行（1 行标题 + 3 行数据）
                Worksheet sheet = wb.Worksheets[0];
                Console.WriteLine($"Total rows loaded: {sheet.Cells.MaxDataRow + 1}");
                Console.WriteLine($"Row 1 (Header): {sheet.Cells[0, 0].StringValue}");
                Console.WriteLine($"Row 2 (Data): {sheet.Cells[1, 0].StringValue}");
                Console.WriteLine($"Row 3 (Data): {sheet.Cells[2, 0].StringValue}");
                Console.WriteLine($"Row 4 (Data): {sheet.Cells[3, 0].StringValue}");

                // 这将为 null，因为我们只加载了 4 行（索引 0-3）
                if (sheet.Cells[4, 0] == null || string.IsNullOrEmpty(sheet.Cells[4, 0].StringValue))
                {
                    Console.WriteLine("Row 5 was not loaded due to MaxRowCount limitation");
                }
            }
        }
    }
}
```

### 另请参见

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


