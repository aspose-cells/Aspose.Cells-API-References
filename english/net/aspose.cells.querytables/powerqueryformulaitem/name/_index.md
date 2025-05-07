---
title: PowerQueryFormulaItem.Name
second_title: Aspose.Cells for .NET API Reference
description: PowerQueryFormulaItem property. Gets the name of the item
type: docs
url: /net/aspose.cells.querytables/powerqueryformulaitem/name/
---
## PowerQueryFormulaItem.Name property

Gets the name of the item.

```csharp
public string Name { get; }
```

### Examples

```csharp
// Called: if (item.Name == "Source")
[Test]
        public void Property_Name()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet47435.xlsx");
            DataMashup mashupData = workbook.DataMashup;
            foreach (PowerQueryFormula formula in mashupData.PowerQueryFormulas)
            {
                foreach (PowerQueryFormulaItem item in formula.PowerQueryFormulaItems)
                {
                    //TestPowerRefresh2
                    if (item.Name == "Source")
                    {
                        item.Value = item.Value.Replace("Parameter1", "\"TESTING\"");
                    }
                }
            }
            //TestPowerRefresh
            //workbook.Worksheets[0].PivotTables[0].RefreshData();

            // Save the output workbookCellsNet47435
            workbook.Save(Constants.destPath + "CellsNet47435.xlsx");
        }
```

### See Also

* class [PowerQueryFormulaItem](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


