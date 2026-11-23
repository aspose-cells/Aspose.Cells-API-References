---
title: "ShapePath.MoveTo"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ShapePath 方法。从指定点开始一个新图形而不关闭当前图形。随后添加到路径的所有点都将加入此新图形。单位: Pixel"
type: docs
url: /zh/net/aspose.cells.drawing/shapepath/moveto/
---
## ShapePath.MoveTo method

从指定点开始一个新图形而不关闭当前图形。随后添加到路径的所有点都将加入此新图形。单位: Pixel。

```csharp
public void MoveTo(float x, float y)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| x | Single | 图形起始点的 x 坐标（单位: Pixel）。 |
| y | Single | 图形起始点的 y 坐标（单位: Pixel）。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodMoveToWithSingleSingleDemo
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

                Console.WriteLine("MoveTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }
           
            
            // 保存结果
            workbook.Save("ShapePathMethodMoveToWithSingleSingleDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


