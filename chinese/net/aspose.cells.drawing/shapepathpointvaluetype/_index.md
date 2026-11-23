---
title: "枚举 ShapePathPointValueType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Drawing.ShapePathPointValueType 枚举。指定 ShapePathPoint 对象的值类型"
type: docs
url: /zh/net/aspose.cells.drawing/shapepathpointvaluetype/
---
## ShapePathPointValueType enumeration

指定 [`ShapePathPoint`](../shapepathpoint/) 对象的值类型

```csharp
public enum ShapePathPointValueType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Position | `0` | 指定对象的类型为位置坐标。[`ShapePathPoint`](../shapepathpoint/) 对象存储点的坐标值。 |
| Angle | `1` | 指定对象的类型为角度标记。[`ShapePathPoint`](../shapepathpoint/) 对象存储弧线的起始和结束角度。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathPointValueTypeDemo
    {
        public static void Run()
        {
            // 创建一个用于演示的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // 演示 ShapePathPointValueType 枚举值
                ShapePathPointValueType positionType = ShapePathPointValueType.Position;
                ShapePathPointValueType angleType = ShapePathPointValueType.Angle;

                // 显示枚举值
                Console.WriteLine($"Position type value: {(int)positionType}");
                Console.WriteLine($"Angle type value: {(int)angleType}");

                // 验证枚举值是否匹配预期常量
                Console.WriteLine($"Position equals 0: {positionType == ShapePathPointValueType.Position}");
                Console.WriteLine($"Angle equals 1: {angleType == ShapePathPointValueType.Angle}");

                Console.WriteLine("ShapePathPointValueType enum demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathPointValueType: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


