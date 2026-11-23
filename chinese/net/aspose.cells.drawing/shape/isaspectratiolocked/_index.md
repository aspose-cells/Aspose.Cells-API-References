---
title: "Shape.IsAspectRatioLocked"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Shape 属性。True 表示形状的宽高比已锁定"
type: docs
url: /zh/net/aspose.cells.drawing/shape/isaspectratiolocked/
---
## Shape.IsAspectRatioLocked property

True 表示形状的宽高比已锁定。

```csharp
public bool IsAspectRatioLocked { get; set; }
```

### 备注

仅适用于图片和 Ole 对象。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsAspectRatioLockedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 50);
            
            Console.WriteLine("Original Aspect Ratio Locked: " + shape.IsAspectRatioLocked);
            
            shape.IsAspectRatioLocked = true;
            Console.WriteLine("After setting to true: " + shape.IsAspectRatioLocked);
            
            shape.IsAspectRatioLocked = false;
            Console.WriteLine("After setting to false: " + shape.IsAspectRatioLocked);
        }
    }
}
```

### 另请参见

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


