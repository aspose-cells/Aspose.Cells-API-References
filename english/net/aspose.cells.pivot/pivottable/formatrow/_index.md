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
            string filePath = Constants.PivotTableSourcePath + @&quot;JAVA44628_&quot;;
            string savePath = CreateFolder(filePath);

            Workbook wb = new Workbook(filePath + &quot;State Reconciliation.xlsx&quot;);
            Worksheet worksheet = wb.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            //Find the cell containing the row field text/label
            Cell cell = worksheet.Cells.Find(&quot;State Apport. Factor&quot;, null);

            //Create the style with your desired formatting
            Style style = wb.CreateStyle();
            style.Custom = &quot;0.00%&quot;;
            style.Font.Name = &quot;Calibri&quot;;
            style.Font.Size = 11;

            //format the row data
            pivotTable.FormatRow(cell.Row, style);

            cell = worksheet.Cells.Find(&quot;Marginal Tax Rate&quot;, null);
            //format the row data
            pivotTable.FormatRow(cell.Row, style);

            wb.Save(savePath + &quot;out.xlsx&quot;);

            string pivotXml = GetEntryText(savePath + &quot;out.xlsx&quot;, @&quot;xl\pivotTables\pivotTable1.xml&quot;);
            Assert.AreNotEqual(pivotXml.IndexOf(&quot;&lt;x v=\&quot;6\&quot; /&gt;&quot;), -1);
            Assert.AreNotEqual(pivotXml.IndexOf(&quot;&lt;x v=\&quot;13\&quot; /&gt;&quot;), -1);

            
        }
```

### See Also

* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


