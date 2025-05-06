---
title: Worksheet.ActiveCell
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets or sets the active cell in the worksheet
type: docs
url: /net/aspose.cells/worksheet/activecell/
---
## Worksheet.ActiveCell property

Gets or sets the active cell in the worksheet.

```csharp
public string ActiveCell { get; set; }
```

### Examples

```csharp
// Called: selectedSheet.ActiveCell = &amp;quot;A1&amp;quot;;
[Test]
        public void Property_ActiveCell()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET45447_&quot;;

            Workbook workbook = new Workbook(filePath + @&quot;template.xlsm&quot;);
            Worksheet selectedSheet = workbook.Worksheets[&quot;Data&quot;];

            DataTable dt = new DataTable();
            dt.ReadXml(filePath + @&quot;b56e4482-836b-415a-ac25-3cb62fc8c5b8.xml&quot;);
            selectedSheet.Cells.ImportData(dt, 1, 0, new ImportTableOptions() { IsFieldNameShown = false });

            selectedSheet = workbook.Worksheets[&quot;Exposure&quot;];
            workbook.Worksheets.ActiveSheetIndex = selectedSheet.Index;
            selectedSheet.ActiveCell = &quot;A1&quot;;
            int iIndex = selectedSheet.PivotTables.Add(&quot;=&apos;Data&apos;!A1:CP43&quot;, &quot;A5&quot;, &quot;IRIS010_pivot&quot;);
            PivotTable selectedPivotTable = selectedSheet.PivotTables[iIndex];

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Column, &quot;Cur&quot;);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Vitol Co&quot;);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Hedge Status&quot;);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Hedge&quot;);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Hedge Name&quot;);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Data, &quot;Amount&quot;);

            selectedPivotTable.RefreshData();
            selectedPivotTable.CalculateRange();
            selectedPivotTable.CalculateData();

            workbook.Save(Constants.PIVOT_CHECK_FILE_PATH + @&quot;NET45447.xlsx&quot;);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


