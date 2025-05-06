---
title: PivotTable.PageFieldOrder
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets and sets the order in which page fields are added to the PivotTable reports layout
type: docs
url: /net/aspose.cells.pivot/pivottable/pagefieldorder/
---
## PivotTable.PageFieldOrder property

Gets and sets the order in which page fields are added to the PivotTable report's layout.

```csharp
public PrintOrderType PageFieldOrder { get; set; }
```

### Examples

```csharp
// Called: pivotTable.PageFieldOrder = PrintOrderType.DownThenOver;
[Test]
        public void Property_PageFieldOrder()
        {
            Aspose.Cells.License license = new Aspose.Cells.License();
            license.SetLicense(Constants.licPath);

            var workbook = new Workbook();
            //Obtaining the reference of the first worksheet
            var sheet = workbook.Worksheets[0];
            //Name the sheet
            sheet.Name = &quot;data&quot;;
            var cells = sheet.Cells;
            int urange = 1;

            cells[&quot;A&quot; + urange].PutValue(&quot;State&quot;);
            cells[&quot;B&quot; + urange].PutValue(&quot;City&quot;);
            cells[&quot;C&quot; + urange].PutValue(&quot;Population&quot;);

            urange++;
            cells[&quot;A&quot; + urange].PutValue(&quot;TN&quot;);
            cells[&quot;B&quot; + urange].PutValue(&quot;Chennai&quot;);
            cells[&quot;C&quot; + urange].PutValue(&quot;50&quot;);

            urange++;
            cells[&quot;A&quot; + urange].PutValue(&quot;KL&quot;);
            cells[&quot;B&quot; + urange].PutValue(&quot;Cochin&quot;);
            cells[&quot;C&quot; + urange].PutValue(&quot;70&quot;);

            urange++;
            cells[&quot;A&quot; + urange].PutValue(&quot;KA&quot;);
            cells[&quot;B&quot; + urange].PutValue(&quot;Bangalore&quot;);
            cells[&quot;C&quot; + urange].PutValue(&quot;80&quot;);

            urange++;
            cells[&quot;A&quot; + urange].PutValue(&quot;AP&quot;);
            cells[&quot;B&quot; + urange].PutValue(&quot;Hydrapad&quot;);
            cells[&quot;C&quot; + urange].PutValue(&quot;63&quot;);

            var listObject = sheet.ListObjects[sheet.ListObjects.Add(&quot;A1&quot;, &quot;C5&quot;, true)];

            //To fit the column as per test size.
            sheet.AutoFitColumns(0, 26);

            //Adding Default Style to the table

            listObject.TableStyleType = TableStyleType.None;

            var sheet2 = workbook.Worksheets[workbook.Worksheets.Add()];

            //Naming the sheet
            sheet2.Name = &quot;PivotSheet&quot;;

            //Getting the pivottables collection in the sheet
            var pivotTables = sheet2.PivotTables;
            //Adding a PivotTable to the worksheet
            var index = pivotTables.Add(&quot;=&quot; + sheet.Name + &quot;!A1:C5&quot;, &quot;A1&quot;, sheet2.Name);

            //To fit the column as per test size.
            sheet2.AutoFitColumns(0, 24);

            //Accessing the instance of the newly added PivotTable
            PivotTable pivotTable = pivotTables[index];

            //Showing the grand totals
            pivotTable.ShowRowGrandTotals = false;
            pivotTable.ShowColumnGrandTotals = false;
            pivotTable.IsAutoFormat = true;

            pivotTable.RowHeaderCaption = &quot;State&quot;;
            pivotTable.AutoFormatType = PivotTableAutoFormatType.None;
            pivotTable.PageFieldOrder = PrintOrderType.DownThenOver;
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight1;

            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;State&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;City&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Data, &quot;Population&quot;);

            var pivotFields = pivotTable.RowFields;

            //Hide the subtotal.
            for (var i = 0; i &lt; pivotFields.Count; i++)
            {
                pivotTable.RowFields[i].SetSubtotals(PivotFieldSubtotalType.None, true);
            }
            sheet2.MoveTo(0);//Move PivotTable Sheets to 0th Position in the workbook

            //for auto-testing
            int activeIndex = -1;
            for (int i = 0; i &lt; workbook.Worksheets.Count; i++)
            {
                if (workbook.Worksheets[i].IsSelected)
                {
                    activeIndex = i;
                    break;
                }
            }
            Assert.AreNotEqual(activeIndex, -1);
            Assert.AreEqual(workbook.Worksheets.ActiveSheetIndex, activeIndex);
            //end

            workbook.Save(Constants.PivotTableDestPath + @&quot;NET43070.xlsx&quot;, SaveFormat.Xlsx);
        }
```

### See Also

* enum [PrintOrderType](../../../aspose.cells/printordertype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


