---
title: OdsLoadOptions.RefreshPivotTables
second_title: Aspose.Cells for .NET API Reference
description: OdsLoadOptions property. Indicates whether refresh pivot tables when loading file
type: docs
url: /net/aspose.cells/odsloadoptions/refreshpivottables/
---
## OdsLoadOptions.RefreshPivotTables property

Indicates whether refresh pivot tables when loading file.

```csharp
public bool RefreshPivotTables { get; set; }
```

### Examples

```csharp
// Called: loadOptions.RefreshPivotTables = true;
[Test]
        public void Property_RefreshPivotTables()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Obtaining the reference of the newly added worksheet
            Worksheet sheet = workbook.Worksheets[0];

            Cells cells = sheet.Cells;

            // Setting the value to the cells
            Cell cell = cells[&quot;A1&quot;];
            cell.PutValue(&quot;Sport&quot;);
            cell = cells[&quot;B1&quot;];
            cell.PutValue(&quot;Quarter&quot;);
            cell = cells[&quot;C1&quot;];
            cell.PutValue(&quot;Sales&quot;);

            cell = cells[&quot;A2&quot;];
            cell.PutValue(&quot;Golf&quot;);
            cell = cells[&quot;A3&quot;];
            cell.PutValue(&quot;Golf&quot;);
            cell = cells[&quot;A4&quot;];
            cell.PutValue(&quot;Tennis&quot;);
            cell = cells[&quot;A5&quot;];
            cell.PutValue(&quot;Tennis&quot;);
            cell = cells[&quot;A6&quot;];
            cell.PutValue(&quot;Tennis&quot;);
            cell = cells[&quot;A7&quot;];
            cell.PutValue(&quot;Tennis&quot;);
            cell = cells[&quot;A8&quot;];
            cell.PutValue(&quot;Golf&quot;);

            cell = cells[&quot;B2&quot;];
            cell.PutValue(&quot;Qtr3&quot;);
            cell = cells[&quot;B3&quot;];
            cell.PutValue(&quot;Qtr4&quot;);
            cell = cells[&quot;B4&quot;];
            cell.PutValue(&quot;Qtr3&quot;);
            cell = cells[&quot;B5&quot;];
            cell.PutValue(&quot;Qtr4&quot;);
            cell = cells[&quot;B6&quot;];
            cell.PutValue(&quot;Qtr3&quot;);
            cell = cells[&quot;B7&quot;];
            cell.PutValue(&quot;Qtr4&quot;);
            cell = cells[&quot;B8&quot;];
            cell.PutValue(&quot;Qtr3&quot;);

            cell = cells[&quot;C2&quot;];
            cell.PutValue(1500);
            cell = cells[&quot;C3&quot;];
            cell.PutValue(2000);
            cell = cells[&quot;C4&quot;];
            cell.PutValue(600);
            cell = cells[&quot;C5&quot;];
            cell.PutValue(1500);
            cell = cells[&quot;C6&quot;];
            cell.PutValue(4070);
            cell = cells[&quot;C7&quot;];
            cell.PutValue(5000);
            cell = cells[&quot;C8&quot;];
            cell.PutValue(6430);

            Aspose.Cells.Pivot.PivotTableCollection pivotTables = sheet.PivotTables;

            // Adding a PivotTable to the worksheet
            int index = pivotTables.Add(&quot;=A1:C8&quot;, &quot;E3&quot;, &quot;PivotTable2&quot;);

            // Accessing the instance of the newly added PivotTable
            Aspose.Cells.Pivot.PivotTable pivotTable = pivotTables[index];

            // Unshowing grand totals for rows.
            pivotTable.ShowRowGrandTotals = false;

            // Draging the first field to the row area.
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0);

            // Draging the second field to the column area.
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, 1);

            // Draging the third field to the data area.
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 2);

            // Saving the Excel file
            //   workbook.Save(&quot;pivotTable_test_out.xls&quot;);
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf11;
            workbook.Save(Constants.destPath + &quot;CellsNet47445.ods&quot;);
            OdsLoadOptions loadOptions = new OdsLoadOptions();
            loadOptions.RefreshPivotTables = true;

            workbook = new Workbook(Constants.destPath + &quot;CellsNet47445.ods&quot;, loadOptions);
            Assert.AreEqual(1, workbook.Worksheets[0].PivotTables.Count);
            workbook.Save(Constants.destPath + &quot;CellsNet47445.ods&quot;);
        }
```

### See Also

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


