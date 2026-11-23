---
title: "TxtLoadOptions.HeaderColumnsCount"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TxtLoadOptions 属性。扩展工作表中要重复的标题列数"
type: docs
url: /zh/net/aspose.cells/txtloadoptions/headercolumnscount/
---
## TxtLoadOptions.HeaderColumnsCount property

扩展工作表中要重复的标题列数。

```csharp
public int HeaderColumnsCount { get; set; }
```

### 备注

此属性指定的标题列将在这些扩展工作表中被复制。仅当 [`ExtendToNextSheet`](../extendtonextsheet/) 为 true 时，此属性才生效。

### 示例

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHeaderColumnsCountDemo
    {
        public static void Run()
        {
            // 创建示例 CSV 内容
            string csvData = "Header1,Header2,Header3,Data1,Data2,Data3\n" +
                            "H1,H2,H3,D1,D2,D3\n" +
                            "A,B,C,D,E,F\n" +
                            "G,H,I,J,K,L";

            // 创建 TxtLoadOptions 并将 HeaderColumnsCount 设置为 3
            TxtLoadOptions options = new TxtLoadOptions
            {
                HeaderColumnsCount = 3, // First 3 columns will be treated as headers
                Encoding = Encoding.UTF8
            };

            // 将 CSV 数据加载到工作簿中
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(csvData)))
            {
                Workbook workbook = new Workbook(stream, options);
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // 演示标题列（前 3 列）
                Console.WriteLine("Header Columns:");
                for (int row = 0; row < 2; row++)
                {
                    for (int col = 0; col < options.HeaderColumnsCount; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
                }

                // 演示数据列（其余列）
                Console.WriteLine("\nData Columns:");
                for (int row = 0; row < cells.MaxDataRow + 1; row++)
                {
                    for (int col = options.HeaderColumnsCount; col < cells.MaxDataColumn + 1; col++)
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


