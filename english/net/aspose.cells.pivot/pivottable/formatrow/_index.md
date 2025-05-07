---
title: PivotTable.FormatRow
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Format the row data in the pivottable area
type: docs
url: /net/aspose.cells.pivot/pivottable/formatrow/
---
## PivotTable.FormatRow method

Format the row data in the pivottable area

```csharp
public void FormatRow(int row, Style style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row Index of the Row object |
| style | Style | Style which is to format |

### Examples

```csharp
// Called: pivotTable.FormatRow(cell.Row, style);
[Test]
        public void Method_Style_()
        {
            string filePath = Constants.PivotTableSourcePath + @"JAVA44632_";

            Workbook wb = new Workbook(filePath + "a.xlsx");
            Worksheet worksheet = wb.Worksheets[1];
            PivotTable pivotTable = worksheet.PivotTables[0];
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            //Create the style with your desired formatting
            Style style = wb.CreateStyle();
            style.Custom = "0.00%";
            style.Font.Name = "Calibri";
            style.Font.Size = 11;

            //Find the cell containing the row field text/label
            Cell cell = worksheet.Cells.Find("Other Adj.", null);

            pivotTable.FormatRow(cell.Row, style);

            cell = worksheet.Cells.Find("Grand Total", null);
            pivotTable.FormatRow(cell.Row, style);
            wb.Save(Constants.PivotTableDestPath + "JAVA44632.html");
            Assert.AreNotEqual(worksheet.Cells["B8"].StringValue.IndexOf("%"), -1);
            Assert.AreNotEqual(worksheet.Cells["B48"].StringValue.IndexOf("%"), -1);
         
        }
```

### See Also

* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


