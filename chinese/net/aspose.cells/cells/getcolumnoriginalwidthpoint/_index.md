---
title: "Cells.GetColumnOriginalWidthPoint"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Cells 方法。获取隐藏列的原始高度，单位为点"
type: docs
url: /zh/net/aspose.cells/cells/getcolumnoriginalwidthpoint/
---
## Cells.GetColumnOriginalWidthPoint method

获取隐藏列的原始高度，单位为点

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetColumnOriginalWidthPoint(int column)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | Int32 | 行索引。 |

### 返回值

普通视图下列的宽度。

### 备注

注意：此方法已过时。请改用 Cells.GetColumnWidth(int ,bool , CellsUnitType ) 方法。该方法将在自2024年4月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnOriginalWidthPointWithInt32Demo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // 准备列索引参数
            int columnIndex = 0;

            try
            {
                // 获取列的原始宽度（单位：点）
                double originalWidth = cells.GetColumnOriginalWidthPoint(columnIndex);
                Console.WriteLine($"Original width of column {columnIndex}: {originalWidth} points");

                // 修改列宽度
                cells.SetColumnWidth(columnIndex, 15);
                Console.WriteLine("Set new column width to 15 points");

                // 再次获取原始宽度以演示其保持不变
                double unchangedWidth = cells.GetColumnOriginalWidthPoint(columnIndex);
                Console.WriteLine($"Original width remains: {unchangedWidth} points");

                // 获取当前宽度以显示修改
                double currentWidth = cells.GetColumnWidth(columnIndex);
                Console.WriteLine($"Current column width: {currentWidth} points");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnOriginalWidthPoint method: {ex.Message}");
            }

            // 保存已修改的工作簿
            workbook.Save("GetColumnOriginalWidthPointDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


