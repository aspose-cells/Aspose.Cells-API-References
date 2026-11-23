---
title: "ShapePath.LineTo"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ShapePath 方法。向当前图形追加一条线段。起始点是当前图形的结束点。单位 像素"
type: docs
url: /zh/net/aspose.cells.drawing/shapepath/lineto/
---
## ShapePath.LineTo method

向当前图形追加一条线段。起始点是当前图形的结束点。单位：像素。

```csharp
public void LineTo(float x, float y)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| x | Single | 线段终点的 x 坐标（单位：像素）。 |
| y | Single | 线段终点的 y 坐标（单位：像素）。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodLineToWithSingleSingleDemo
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

                // 移动到起始点
                shapePath.MoveTo(10, 10);
                
                // 使用 (Single, Single) 参数调用 LineTo 方法
                shapePath.LineTo(50.5f, 10.5f);
                shapePath.LineTo(50.5f, 50.5f);
                shapePath.LineTo(10.5f, 50.5f);
                shapePath.Close();

                //添加自由形状
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                Console.WriteLine("LineTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }
            
            // 保存结果
            workbook.Save("ShapePathMethodLineToWithSingleSingleDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


