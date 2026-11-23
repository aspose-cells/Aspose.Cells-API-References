---
title: "Shape.IsDecorative"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Shape 属性。指示对象是否为装饰性"
type: docs
url: /zh/net/aspose.cells.drawing/shape/isdecorative/
---
## Shape.IsDecorative property

指示对象是否为装饰性。

```csharp
public bool IsDecorative { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsDecorativeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加矩形形状
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            
            // 将形状设为装饰性
            shape.IsDecorative = true;
            
            // 保存工作簿
            string outputPath = "ShapeIsDecorativeDemo.xlsx";
            workbook.Save(outputPath);
            
            // 重新加载工作簿以验证该属性
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            
            // 输出结果
            Console.WriteLine("Shape IsDecorative property: " + loadedShape.IsDecorative);
        }
    }
}
```

### 另请参见

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


