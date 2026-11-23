---
title: "枚举 CellsUnitType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.CellsUnitType 枚举。指定测量单位"
type: docs
url: /zh/net/aspose.cells/cellsunittype/
---
## CellsUnitType enumeration

指定测量单位。

```csharp
public enum CellsUnitType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Pixel | `1` | 测量单位为像素。 |
| Point | `2` | 测量单位为点。1 点等于 1/72 英寸。 |
| Inch | `4` | 测量单位为英寸。 |
| Cm | `6` | 测量单位为厘米。 |
| Character | `7` | 以字符为单位。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCellsUnitTypeDemo
    {
        public static void Run()
        {
            // 创建一个用于演示的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // 演示使用不同的 CellsUnitType 枚举值
                Console.WriteLine("Available CellsUnitType values:");

                // 显示所有枚举值
                Console.WriteLine("Pixel: " + CellsUnitType.Pixel);
                Console.WriteLine("Point: " + CellsUnitType.Point);
                Console.WriteLine("Inch: " + CellsUnitType.Inch);
                Console.WriteLine("Cm: " + CellsUnitType.Cm);
                Console.WriteLine("Character: " + CellsUnitType.Character);

                // 示例用法：使用不同单位设置列宽
                worksheet.Cells.SetColumnWidthPixel(0, 100); // Using Pixel unit
                worksheet.Cells.SetColumnWidthInch(1, 2.0);  // Using Inch unit

                // 保存工作簿以演示完整流程
                workbook.Save("CellsUnitTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with different unit types applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with CellsUnitType: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


