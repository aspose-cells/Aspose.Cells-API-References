---
title: "PivotTableFormatCollection.FormatArea"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotTableFormatCollection 方法。格式化选定区域"
type: docs
url: /zh/net/aspose.cells.pivot/pivottableformatcollection/formatarea/
---
## PivotTableFormatCollection.FormatArea method

格式化选定区域。

```csharp
public PivotTableFormat FormatArea(PivotFieldType axisType, int fieldPosition, 
    PivotFieldSubtotalType subtotalType, PivotTableSelectionType selectionType, bool isGrandRow, 
    bool isGrandColumn, Style style)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| axisType | PivotFieldType | 此规则适用的透视表区域。 |
| fieldPosition | Int32 | 此规则适用的轴上字段的位置。 |
| subtotalType | PivotFieldSubtotalType | 透视字段的子总计过滤类型 |
| selectionType | PivotTableSelectionType | 指示如何选择数据。 |
| isGrandRow | 布尔 | 指示是否选择总计行。 |
| isGrandColumn | 布尔 | 指示是否选择总计列。 |
| 样式 | 样式 | 应用于数据透视表区域的样式。 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotTableFormatCollectionMethodFormatAreaWithPivotFieldTypeInt32PivotFieldSDemo
    {
        public static void Run()
        {
            // 从源文件创建工作簿
            Workbook workbook = new Workbook("example.xlsx");
            
            // 访问数据透视表
            PivotTable pt = workbook.Worksheets["PIVOT_VBA_SUBTOTALS"].PivotTables[0];
            
            // 创建用于格式化的样式
            Style style = workbook.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Red);
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.LightGray;
            style.BackgroundColor = Color.LightGray;

            // 格式化数据透视表区域
            pt.PivotFormats.FormatArea(
                PivotFieldType.Row, 
                0, 
                PivotFieldSubtotalType.Automatic, 
                PivotTableSelectionType.DataAndLabel, 
                false, 
                false, 
                style);

            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotTableFormat](../../pivottableformat/)
* enum [PivotFieldType](../../pivotfieldtype/)
* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* enum [PivotTableSelectionType](../../pivottableselectiontype/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTableFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


