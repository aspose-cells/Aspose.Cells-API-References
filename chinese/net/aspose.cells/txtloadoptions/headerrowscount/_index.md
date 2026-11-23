---
title: "TxtLoadOptions.HeaderRowsCount"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TxtLoadOptions 属性。要在扩展工作表中重复的标题行数"
type: docs
url: /zh/net/aspose.cells/txtloadoptions/headerrowscount/
---
## TxtLoadOptions.HeaderRowsCount property

要在扩展工作表中重复的标题行数。

```csharp
public int HeaderRowsCount { get; set; }
```

### 备注

此属性指定的标题行将在这些扩展工作表中被复制。仅当 [`ExtendToNextSheet`](../extendtonextsheet/) 为 true 时，此属性才生效。

### 示例

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHeaderRowsCountDemo
    {
        public static void Run()
        {
            // 创建示例 CSV 内容
            string csvData = "Header1,Header2,Header3\n" +
                            "Value1,Value2,Value3\n" +
                            "Value4,Value5,Value6\n" +
                            "Value7,Value8,Value9";

            // 创建 TxtLoadOptions 并将 HeaderRowsCount 设置为 1
            TxtLoadOptions options = new TxtLoadOptions
            {
                HeaderRowsCount = 1
            };

            // 将 CSV 数据加载到工作簿中
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(csvData)))
            {
                Workbook workbook = new Workbook(stream, options);

                // 访问第一个工作表
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // 演示第一行被视为标题
                Console.WriteLine("Header Row:");
                for (int col = 0; col < cells.MaxDataColumn + 1; col++)
                {
                    Console.Write(cells[0, col].StringValue + "\t");
                }
                Console.WriteLine("\n");

                // 显示数据行（跳过标题）
                Console.WriteLine("Data Rows:");
                for (int row = 1; row < cells.MaxDataRow + 1; row++)
                {
                    for (int col = 0; col < cells.MaxDataColumn + 1; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
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


