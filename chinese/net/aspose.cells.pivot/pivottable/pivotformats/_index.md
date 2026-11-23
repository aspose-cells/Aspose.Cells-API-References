---
title: "PivotTable.PivotFormats"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotTable 属性。获取应用于此数据透视表的所有单元格格式"
type: docs
url: /zh/net/aspose.cells.pivot/pivottable/pivotformats/
---
## PivotTable.PivotFormats property

获取应用于此数据透视表的所有单元格格式。

```csharp
public PivotTableFormatCollection PivotFormats { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPivotFormatsDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // 为数据透视表添加示例数据
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["B1"].Value = "Quantity";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["B2"].Value = 10;
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["B3"].Value = 15;
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B4"].Value = 20;

            // 创建数据透视表
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // 创建用于格式化的样式
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.LightBlue;
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, System.Drawing.Color.Black);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, System.Drawing.Color.Black);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, System.Drawing.Color.Black);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, System.Drawing.Color.Black);

            // 将格式应用于数据透视表数据区域
            pivotTable.PivotFormats.FormatArea(
                PivotFieldType.Data, 
                0, 
                PivotFieldSubtotalType.None, 
                PivotTableSelectionType.DataAndLabel, 
                false, 
                false, 
                style);

            // 保存工作簿
            workbook.Save("PivotTableWithFormats.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotTableFormatCollection](../../pivottableformatcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


