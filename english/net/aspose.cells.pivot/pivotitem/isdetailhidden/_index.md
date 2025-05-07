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
// Called: pivotTable.RowFields[0].PivotItems["State Apport. Factor"].IsDetailHidden = false;
[Test]
        public void Property_IsDetailHidden()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET50356_";
            string savePath = CreateFolder(filePath);

            Workbook wb = new Workbook(filePath + "State Reconciliation.xlsx");
            Worksheet worksheet = wb.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            //Find the cell containing the row field text/label
            Cell cell = worksheet.Cells.Find("State Apport. Factor", null);

            //Create the style with your desired formatting
            Style style = wb.CreateStyle();
            style.Custom = "0.00%";
            style.Font.Name = "Calibri";
            style.Font.Size = 11;


            //Get the row index
            int row = cell.Row;

            //Get the cell area based on pivot table range
            CellArea area = pivotTable.TableRange1;
            //Get the starting column index
            int start = area.StartColumn;

            //browse the relevant row upto last column in the pivot table report
            //format each cell in the row to set percentage numbers formatting
            for (int i = start; i <= area.EndColumn; i++)
            {
                pivotTable.Format(row, i, style);
            }

            //Change the state of PivotItem
            pivotTable.RowFields[0].PivotItems["State Apport. Factor"].IsDetailHidden = false;
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            //After expanding the data, format it again
            for (int i = start; i <= area.EndColumn; i++)
            {
                pivotTable.Format(row, i, style);
            }
            //Restore previous state
            pivotTable.RowFields[0].PivotItems["State Apport. Factor"].IsDetailHidden = true;

            wb.Save(savePath + "out.xlsx");

            Assert.AreEqual(worksheet.Cells["C22"].StringValue, "100.00%");
            Assert.AreEqual(worksheet.Cells["F22"].StringValue, "19.28%");
        }
```

### See Also

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


