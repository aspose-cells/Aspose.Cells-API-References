---
title: PivotTable.RowHeaderCaption
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets the Row Header Caption of the PivotTable
type: docs
url: /net/aspose.cells.pivot/pivottable/rowheadercaption/
---
## PivotTable.RowHeaderCaption property

Gets the Row Header Caption of the PivotTable.

```csharp
public string RowHeaderCaption { get; set; }
```

### Examples

```csharp
// Called: pivotTable.RowHeaderCaption = &amp;quot;ID&amp;quot;;
[Test]
        public void Property_RowHeaderCaption()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CellsNet55115.xlsx&quot;);
            Worksheet worksheet = workbook.Worksheets[0];
            int maxdatacol = worksheet.Cells.MaxDataColumn;
            int maxdatarow = worksheet.Cells.MaxDataRow;
            string cellname = CellsHelper.CellIndexToName(maxdatarow, maxdatacol);

            Worksheet pivotSheet = workbook.Worksheets[workbook.Worksheets.Add()];
            Column column = pivotSheet.Cells.Columns[1];
            //Style style = column.GetStyle();
            //style.Number = 14;
            //column.SetStyle(style);

            PivotTable pivotTable = pivotSheet.PivotTables[pivotSheet.PivotTables.Add(&quot;=&quot; + worksheet.Name + &quot;!A1:&quot; + cellname, &quot;A1&quot;, &quot;PivotTable1&quot;)];

            pivotTable.ShowRowGrandTotals = false;
            pivotTable.ShowColumnGrandTotals = false;
            pivotTable.ShowDrill = false;

            pivotTable.RowHeaderCaption = &quot;ID&quot;;
            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;ID&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Date Created&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Type&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;PayAmount&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Column, &quot;PivotColumn&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Data, &quot;Value&quot;);

            for (int i = 0; i &lt; pivotTable.RowFields.Count; i++)
            {
                pivotTable.RowFields[i].SetSubtotals(PivotFieldSubtotalType.None, true);
                pivotTable.RowFields[i].IsRepeatItemLabels = true;
            }
          

            pivotTable.AutoFormatType = PivotTableAutoFormatType.None;
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Worksheet copySheet = workbook.Worksheets[workbook.Worksheets.Add()];

            copySheet.Cells.CopyRows(pivotSheet.Cells, 1, 0, pivotSheet.Cells.MaxDataRow);

            Assert.AreEqual(&quot;12/17/2023&quot;, copySheet.Cells[&quot;B4&quot;].StringValue);

            workbook.Save(Constants.PivotTableDestPath + &quot;CellsNet55115.xlsx&quot;);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


