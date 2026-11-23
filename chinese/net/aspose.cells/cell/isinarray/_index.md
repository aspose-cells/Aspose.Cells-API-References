---
title: "Cell.IsInArray"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Cell 属性。指示单元格公式是否为数组公式"
type: docs
url: /zh/net/aspose.cells/cell/isinarray/
---
## Cell.IsInArray property

指示单元格公式是否为数组公式。

```csharp
[Obsolete("Use IsArrayFormula instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsInArray { get; }
```

### 备注

注意：此类已过时。请改用 Cell.IsArrayFormula 来检查单元格公式是否为数组公式。此属性将在自 2018 年 5 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsInArrayDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建带有数组公式的示例数据
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // 使用正确的 API 设置数组公式
            worksheet.Cells["C2"].SetArrayFormula("A2:A3*B2:B3", 2, 1);

            // 检查 IsInArray 属性
            Cell cellInArray = worksheet.Cells["C2"];
            Cell cellNotInArray = worksheet.Cells["A2"];

            Console.WriteLine("Cell C2 is in array: " + cellInArray.IsInArray);
            Console.WriteLine("Cell A2 is in array: " + cellNotInArray.IsInArray);

            // 演示清除非数组单元格
            for (int row = 1; row <= 3; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Cell cell = worksheet.Cells[row, col];
                    if (!cell.IsInArray && !cell.IsFormula)
                    {
                        cell.PutValue("");
                    }
                }
            }

            // 保存工作簿
            workbook.Save("IsInArrayDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


