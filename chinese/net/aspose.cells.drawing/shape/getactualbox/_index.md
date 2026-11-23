---
title: "Shape.GetActualBox"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Shape 方法。获取在应用旋转、翻转等操作后形状的实际位置和大小"
type: docs
url: /zh/net/aspose.cells.drawing/shape/getactualbox/
---
## Shape.GetActualBox method

获取形状的实际位置和大小（在应用旋转、翻转等操作后）

```csharp
public float[] GetActualBox()
```

### 返回值

返回位置和大小，顺序为 x、y、w、h

### 备注

注意：该接口尚未完全功能化，尤其是位置信息不正确。建议在功能完成之前不要使用此接口。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetActualBoxDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加矩形形状
            Shape rectangle = worksheet.Shapes.AddRectangle(10, 10, 100, 80, 0, 0);

            // 获取形状的实际框尺寸
            float[] box = rectangle.GetActualBox();

            // 输出框尺寸
            Console.WriteLine("Actual Box Dimensions:");
            Console.WriteLine($"Left: {box[0]}");
            Console.WriteLine($"Top: {box[1]}");
            Console.WriteLine($"Right: {box[2]}");
            Console.WriteLine($"Bottom: {box[3]}");

            // 保存工作簿
            workbook.Save("ShapeGetActualBoxDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


