---
title: "PivotTableFormat.SetStyle"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotTableFormat 方法。设置透视区域的样式"
type: docs
url: /zh/net/aspose.cells.pivot/pivottableformat/setstyle/
---
## PivotTableFormat.SetStyle method

设置数据透视区域的样式。

```csharp
public void SetStyle(Style style)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 样式 | 样式 |  |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotTableFormatMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Year";
            worksheet.Cells["C1"].Value = "Amount";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 2020;
            worksheet.Cells["C2"].Value = 50;
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B3"].Value = 2020;
            worksheet.Cells["C3"].Value = 60;

            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2);

            PivotTableFormatCollection formatCollection = pivotTable.PivotFormats;
            int formatIndex = formatCollection.Add();
            PivotTableFormat pivotFormat = formatCollection[formatIndex];

            Style style = workbook.CreateStyle();
            style.BackgroundColor = Color.LightBlue;
            style.Font.Color = Color.DarkBlue;
            style.Font.IsBold = true;

            pivotFormat.SetStyle(style);

            workbook.Save("PivotTableSetStyleDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Style](../../../aspose.cells/style/)
* class [PivotTableFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


