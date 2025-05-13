---
title: PivotField.GetFormula
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Gets formula of the calculated field 
type: docs
url: /net/aspose.cells.pivot/pivotfield/getformula/
---
## PivotField.GetFormula method

Gets formula of the calculated field .

```csharp
public string GetFormula()
```

### Examples

```csharp
// Called: Assert.AreEqual("=ABS('ns1:TRN_AMOUNT')", fields[fields.Count - 1].GetFormula());
public void PivotField_Method_GetFormula()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    PivotFieldCollection fields = workbook.Worksheets[1].PivotTables[0].BaseFields;
    Assert.AreEqual("=ABS('ns1:TRN_AMOUNT')", fields[fields.Count - 1].GetFormula());
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


