---
title: "ShapePath.Close"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ShapePath 方法。关闭当前图形并开始一个新图形。如果当前图形包含一系列相连的直线和曲线，该方法通过从端点连接一条线到起始点来闭合环路。"
type: docs
url: /zh/net/aspose.cells.drawing/shapepath/close/
---
## ShapePath.Close method

关闭当前图形并开始一个新图形。如果当前图形包含一系列相连的直线和曲线，方法通过从端点连接一条线到起始点来闭合环路。

```csharp
public void Close()
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCloseDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                //创建新的形状路径
                ShapePath shapePath = new ShapePath();
                shapePath.MoveTo(60, 45);
                shapePath.ArcTo(25, 25, 0, 270);

                // 关闭路径
                shapePath.Close();

                shapePath.MoveTo(60, 20);
                shapePath.LineTo(110, 70);
                shapePath.LineTo(125, 155.5f);
                shapePath.ArcTo(35.5f, 35.5f, 0, 270);

                // 关闭路径
                shapePath.Close();

                //添加自由形状
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                Console.WriteLine("Close method called successfully to complete the shape path");
                
                // 保存工作簿
                workbook.Save("ShapePathMethodCloseDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Close method: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


