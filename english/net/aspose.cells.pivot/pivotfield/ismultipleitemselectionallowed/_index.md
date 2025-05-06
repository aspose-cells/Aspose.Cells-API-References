---
title: PivotField.IsMultipleItemSelectionAllowed
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. indicates whether the field can have multiple items selected in the page field The default value is false
type: docs
url: /net/aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed/
---
## PivotField.IsMultipleItemSelectionAllowed property

indicates whether the field can have multiple items selected in the page field The default value is false.

```csharp
public bool IsMultipleItemSelectionAllowed { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(wb.Worksheets[0].PivotTables[0].PageFields[0].IsMultipleItemSelectionAllowed);
[Test]
        public void Property_IsMultipleItemSelectionAllowed()
        {
            Workbook wb = new Workbook(Constants.PivotTableSourcePath + &quot;CellsNet49364.xlsx&quot;);

            for (var i = 0; i &lt; wb.Worksheets.Count; i++)
            {

                foreach (PivotTable pivotTable in wb.Worksheets[i].PivotTables)
                {
                    pivotTable.RefreshData();
                    pivotTable.CalculateData();
                }
            }
            Assert.IsFalse(wb.Worksheets[0].PivotTables[0].PageFields[0].IsMultipleItemSelectionAllowed);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;E16&quot;].StringValue, &quot;3,837.60&quot;);
            wb.Save(Constants.PivotTableDestPath + &quot;CellsNet49364.xlsx&quot;, SaveFormat.Xlsx);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


