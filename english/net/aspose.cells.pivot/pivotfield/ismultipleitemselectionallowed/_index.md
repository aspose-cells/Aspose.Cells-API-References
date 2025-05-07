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
// Called: Assert.AreEqual(pivot.PageFields[0].IsMultipleItemSelectionAllowed, true);
[Test]
        public void Property_IsMultipleItemSelectionAllowed()
        {
            Workbook wb = new Workbook(Constants.PivotTableSourcePath + "CELLSNET-53946.xlsx");            

            PivotTable pivot = wb.Worksheets[0].PivotTables["数据透视表18"];

            //NET53948
            Assert.AreEqual(pivot.PageFields[0].IsMultipleItemSelectionAllowed, true);

            wb.Worksheets[0].RefreshPivotTables();

            //NET53946
            Assert.AreEqual(wb.Worksheets[0].Cells["D5"].StringValue, "0.017525878");
            Assert.AreEqual(wb.Worksheets[0].Cells["D9"].StringValue, "0.0214485");
            Assert.IsTrue(string.IsNullOrEmpty(wb.Worksheets[0].Cells["H8"].StringValue));
            //END

            //NET53948
            Assert.AreEqual(pivot.PageFields[0].IsMultipleItemSelectionAllowed, true);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


