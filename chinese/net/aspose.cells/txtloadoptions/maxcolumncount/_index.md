---
title: "TxtLoadOptions.MaxColumnCount"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TxtLoadOptions 属性。每个工作表要导入的最大列数"
type: docs
url: /zh/net/aspose.cells/txtloadoptions/maxcolumncount/
---
## TxtLoadOptions.MaxColumnCount property

每个工作表要导入的最大列数。

```csharp
public int MaxColumnCount { get; set; }
```

### 备注

超过此限制的列将根据 [`ExtendToNextSheet`](../extendtonextsheet/) 被忽略或扩展到下一个工作表。此计数包括标题列（[`HeaderColumnsCount`](../headercolumnscount/)）。它的最大值是相应文件格式的列限制，例如对于 xlsx 文件为 16384。如果未指定此属性或指定的值不是正数，则也将使用最大限制。

### 示例

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyMaxColumnCountDemo
    {
        public static void Run()
        {
            // 创建示例 CSV 内容
            string content = "A,B,C,D,E,F,G,H,I,J,K\n" +
                            "1,2,3,4,5,6,7,8,9,10,11\n" +
                            "a,b,c,d,e,f,g,h,i,j,k";

            // 创建 TxtLoadOptions 并将 MaxColumnCount 设置为 5
            TxtLoadOptions options = new TxtLoadOptions
            {
                MaxColumnCount = 5  // Only load first 5 columns
            };

            // 使用受限列加载 CSV
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(content)))
            {
                Workbook workbook = new Workbook(stream, options);
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // 输出已加载的数据（仅应显示前5列）
                Console.WriteLine("Data loaded with MaxColumnCount = 5:");
                for (int row = 0; row < cells.MaxDataRow + 1; row++)
                {
                    for (int col = 0; col < cells.MaxDataColumn + 1; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
                }

                // 验证仅加载了5列
                Console.WriteLine($"\nMax loaded columns: {cells.MaxDataColumn + 1}");
            }
        }
    }
}
```

### 另请参见

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


