---
title: PowerQueryFormulaItem.Value
second_title: Aspose.Cells for .NET API Reference
description: PowerQueryFormulaItem property. Gets the value of the item
type: docs
url: /net/aspose.cells.querytables/powerqueryformulaitem/value/
---
## PowerQueryFormulaItem.Value property

Gets the value of the item.

```csharp
public string Value { get; set; }
```

### Examples

```csharp
// Called: item.Value = item.Value.Replace("Parameter1", "\"TESTING\"");
public void PowerQueryFormulaItem_Property_Value()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
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
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [PowerQueryFormulaItem](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


