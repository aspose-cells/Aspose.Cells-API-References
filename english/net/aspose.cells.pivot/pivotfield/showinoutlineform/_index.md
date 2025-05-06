---
title: PivotField.ShowInOutlineForm
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether layout this field in outline form on the Pivot Table view
type: docs
url: /net/aspose.cells.pivot/pivotfield/showinoutlineform/
---
## PivotField.ShowInOutlineForm property

Indicates whether layout this field in outline form on the Pivot Table view

```csharp
public bool ShowInOutlineForm { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(pivotTable.DataFields[0].ShowInOutlineForm);
[Test]
        public void Property_ShowInOutlineForm()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET47526_&quot;;

            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Obtaining the reference of the newly added worksheet
            Worksheet sheet = workbook.Worksheets[0];

            Cells cells = sheet.Cells;

            #region  Setting the value to the cells
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
            #endregion

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

            Console.WriteLine(pivotTable.RowFields[0].ShowInOutlineForm);
            Console.WriteLine(pivotTable.ColumnFields[0].ShowInOutlineForm);
            Console.WriteLine(pivotTable.DataFields[0].ShowInOutlineForm);
            Console.WriteLine(pivotTable.DataFields[0].InsertBlankRow);

            workbook.Save(CreateFolder(filePath) + &quot;dest.ods&quot;);

        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


