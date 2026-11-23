---
title: "ShapeTextAlignment.NumberOfColumns"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ShapeTextAlignment 属性。获取并设置边界矩形中文本的列数"
type: docs
url: /zh/net/aspose.cells.drawing.texts/shapetextalignment/numberofcolumns/
---
## ShapeTextAlignment.NumberOfColumns property

获取并设置边界矩形中文本的列数。

```csharp
public int NumberOfColumns { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyNumberOfColumnsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 向工作表添加形状
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);
            
            // 为形状设置文本
            shape.Text = "This is sample text\nin multiple columns";
            
            // 访问文本对齐并设置列数
            shape.TextBody.TextAlignment.NumberOfColumns = 2;
            
            // 保存工作簿
            workbook.Save("output.xlsx");
            
            // 验证属性
            Console.WriteLine("Number of columns: " + 
                worksheet.Shapes[0].TextBody.TextAlignment.NumberOfColumns);
        }
    }
}
```

### 另请参见

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


