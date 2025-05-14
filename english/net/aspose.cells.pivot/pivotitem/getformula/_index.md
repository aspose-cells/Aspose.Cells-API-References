---
title: PivotItem.GetFormula
second_title: Aspose.Cells for .NET API Reference
description: PivotItem method. Gets the formula of this calculated item. Only works when this item is calculated item
type: docs
url: /net/aspose.cells.pivot/pivotitem/getformula/
---
## PivotItem.GetFormula method

Gets the formula of this calculated item. Only works when this item is calculated item.

```csharp
public string GetFormula()
```

### Examples

```csharp
// Called: Assert.AreEqual("='w''e'",wb.Worksheets[0].PivotTables[0].RowFields[0].PivotItems[2].GetFormula());
public void PivotItem_Method_GetFormula()
{

    Workbook wb = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
   Assert.AreEqual("='b''b'",wb.Worksheets[0].PivotTables[0].DataFields[1].GetFormula());
   Assert.AreEqual("='w''e'",wb.Worksheets[0].PivotTables[0].RowFields[0].PivotItems[2].GetFormula());
    wb.Save(Constants.PivotTableDestPath + "example.xlsb");
    wb = new Workbook(Constants.PivotTableDestPath + "example.xlsb");
    Assert.AreEqual("='b''b'", wb.Worksheets[0].PivotTables[0].DataFields[1].GetFormula());
    Assert.AreEqual("='w''e'", wb.Worksheets[0].PivotTables[0].RowFields[0].PivotItems[2].GetFormula());
    wb.Save(Constants.PivotTableDestPath + "example.xlsx");
}
```

### See Also

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


