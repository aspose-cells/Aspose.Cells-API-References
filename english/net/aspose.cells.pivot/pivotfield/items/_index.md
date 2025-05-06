---
title: PivotField.Items
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Get all labels of pivot items in this field
type: docs
url: /net/aspose.cells.pivot/pivotfield/items/
---
## PivotField.Items property

Get all labels of pivot items in this field.

```csharp
public string[] Items { get; }
```

### Examples

```csharp
// Called: string[] items = pivotTable.ColumnFields[0].Items;
[Test]
        public void Property_Items()
        {
            //Instantiating an Workbook object
            Workbook workbook = new Workbook();
            // workbook.Open(@&quot;F:\FileTemp\book2.xls&quot;);
            //

            //Obtaining the reference of the newly added worksheet
            Worksheet sheet = workbook.Worksheets[0];


            Cells cells = sheet.Cells;


            //Setting the value to the cells
            Cell cell = cells[&quot;A1&quot;];
            cell.PutValue(&quot;Sport&quot;);
            cell = cells[&quot;B1&quot;];
            cell.PutValue(&quot;Quarter test&quot;);
            cell = cells[&quot;C1&quot;];
            cell.PutValue(&quot;Sales&quot;);
            cell = cells[&quot;D1&quot;];
            cell.PutValue(&quot;Sales1&quot;);

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

            cell = cells[&quot;D2&quot;];
            cell.PutValue(0);
            cell = cells[&quot;D3&quot;];
            cell.PutValue(0);
            cell = cells[&quot;D4&quot;];
            cell.PutValue(0);
            cell = cells[&quot;D5&quot;];
            cell.PutValue(0);
            cell = cells[&quot;D6&quot;];
            cell.PutValue(0);
            cell = cells[&quot;D7&quot;];
            cell.PutValue(0);
            cell = cells[&quot;D8&quot;];
            cell.PutValue(0);


            cell = cells[&quot;G22&quot;];
            //cell.Style.HorizontalAlignment = TextAlignmentType.Center;

            Style style = cell.GetStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            cell.SetStyle(style);
            

            PivotTableCollection pivotTables = sheet.PivotTables;


            //Adding a PivotTable to the worksheet
            int index = pivotTables.Add(&quot;=A1:D80000&quot;, &quot;E20&quot;, &quot;PivotTable1&quot;);


            //Accessing the instance of the newly added PivotTable
            PivotTable pivotTable = pivotTables[index];
            

            //Unshowing grand totals for rows.
            // pivotTable.RowGrand = false;


            //Draging the first field to the row area.
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);


            //Draging the second field to the column area.
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2);

            string[] items = pivotTable.ColumnFields[0].Items;
            Assert.AreEqual(items[0], &quot;Qtr3&quot;);
            Assert.AreEqual(items[1], &quot;Qtr4&quot;);
            workbook.Save(Constants.PivotTableDestPath + &quot;N43877.xlsx&quot;);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


