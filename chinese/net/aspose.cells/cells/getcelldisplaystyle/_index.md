---
title: "Cells.GetCellDisplayStyle"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Cells 方法。获取给定单元格的显示样式"
type: docs
url: /zh/net/aspose.cells/cells/getcelldisplaystyle/
---
## GetCellDisplayStyle(int, int) {#getcelldisplaystyle}

获取给定单元格的显示样式。

```csharp
public Style GetCellDisplayStyle(int row, int column)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | Int32 | 给定单元格的行索引 |
| 列 | Int32 | 给定单元格的列 |

### 返回值

给定单元格的显示样式。

### 备注

与 [`GetDisplayStyle`](../../cell/getdisplaystyle/) 相同，使用 SideBorders 对 `GetCellDisplayStyle` 也相同。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetCellDisplayStyleWithInt32Int32Demo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // 准备用于演示的单元格样式
            Cell cell = cells[0, 0];
            cell.PutValue("Style Demo");
            
            // 创建自定义样式
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // 将样式应用于单元格
            cell.SetStyle(style);

            try
            {
                // 使用第0行第0列调用 GetCellDisplayStyle
                Style displayStyle = cells.GetCellDisplayStyle(0, 0);

                // 显示样式属性
                Console.WriteLine($"Bold: {displayStyle.Font.IsBold}");
                Console.WriteLine($"Background Color: {displayStyle.ForegroundColor}");

                // 将显示样式应用于另一个单元格以进行可视化验证
                cells[2, 2].SetStyle(displayStyle);
                cells[2, 2].PutValue("Style Copied");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellDisplayStyle method: {ex.Message}");
            }

            // 保存工作簿
            workbook.Save("CellsMethodGetCellDisplayStyleWithInt32Int32Demo.xlsx");
        }
    }
}
```

### 另请参见

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCellDisplayStyle(int, int, BorderType) {#getcelldisplaystyle_1}

获取给定单元格的显示样式。

```csharp
public Style GetCellDisplayStyle(int row, int column, BorderType adjacentBorders)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | Int32 | 给定单元格的行索引 |
| 列 | Int32 | 给定单元格的列 |
| adjacentBorders | BorderType | 指示需要根据相邻单元格的边框检查和调整的边框。请参阅 [`GetDisplayStyle`](../../cell/getdisplaystyle/) 中相同参数的说明。 |

### 返回值

给定单元格的显示样式。

### 备注

如果单元格还受到条件格式、列表对象等其他设置的影响，则显示样式可能与 [`GetCellStyle`](../getcellstyle/) 不同。并且由于这些设置也可能应用于空（不存在的）单元格，使用此方法可以避免实例化这些空单元格，从而性能优于先从 Cells 获取 Cell 实例再调用 [`GetDisplayStyle`](../../cell/getdisplaystyle/)。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetCellDisplayStyleWithInt32Int32BorderTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 访问单元格 A1 并设置边框样式
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            cell.SetStyle(style);

            try
            {
                // 使用特定参数调用 GetCellDisplayStyle（A1 为 (0,0)，TopBorder 类型）
                Style displayStyle = worksheet.Cells.GetCellDisplayStyle(0, 0, BorderType.TopBorder);

                // 检查检索到的样式是否与我们的边框颜色匹配
                if (displayStyle.Borders[BorderType.TopBorder].Color == System.Drawing.Color.Red)
                {
                    Console.WriteLine("Top border display style retrieved successfully - Color: Red");
                }

                // 通过修改另一个单元格演示样式的应用
                Cell targetCell = worksheet.Cells["B1"];
                targetCell.SetStyle(displayStyle);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellDisplayStyle method: {ex.Message}");
            }

            // 保存结果
            workbook.Save("GetCellDisplayStyleWithBorderTypeDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


