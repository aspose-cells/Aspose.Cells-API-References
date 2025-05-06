---
title: PivotItem.IsDetailHidden
second_title: Aspose.Cells for .NET API Reference
description: PivotItem property. Gets and sets whether the detail of this pivot item is hidden
type: docs
url: /net/aspose.cells.pivot/pivotitem/isdetailhidden/
---
## PivotItem.IsDetailHidden property

Gets and sets whether the detail of this pivot item is hidden.

```csharp
public bool IsDetailHidden { get; set; }
```

### Examples

```csharp
// Called: pivotTable.RowFields[0].PivotItems[&amp;quot;State Apport. Factor&amp;quot;].IsDetailHidden = false;
[Test]
        public void Property_IsDetailHidden()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET50356_&quot;;
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


            //Get the row index
            int row = cell.Row;

            //Get the cell area based on pivot table range
            CellArea area = pivotTable.TableRange1;
            //Get the starting column index
            int start = area.StartColumn;

            //browse the relevant row upto last column in the pivot table report
            //format each cell in the row to set percentage numbers formatting
            for (int i = start; i &lt;= area.EndColumn; i++)
            {
                pivotTable.Format(row, i, style);
            }

            //Change the state of PivotItem
            pivotTable.RowFields[0].PivotItems[&quot;State Apport. Factor&quot;].IsDetailHidden = false;
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            //After expanding the data, format it again
            for (int i = start; i &lt;= area.EndColumn; i++)
            {
                pivotTable.Format(row, i, style);
            }
            //Restore previous state
            pivotTable.RowFields[0].PivotItems[&quot;State Apport. Factor&quot;].IsDetailHidden = true;

            wb.Save(savePath + &quot;out.xlsx&quot;);

            Assert.AreEqual(worksheet.Cells[&quot;C22&quot;].StringValue, &quot;100.00%&quot;);
            Assert.AreEqual(worksheet.Cells[&quot;F22&quot;].StringValue, &quot;19.28%&quot;);
        }
```

### See Also

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


