---
title: PowerQueryFormula.PowerQueryFormulaItems
second_title: Aspose.Cells for .NET API Reference
description: PowerQueryFormula property. Gets all items of power query formula
type: docs
url: /net/aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/
---
## PowerQueryFormula.PowerQueryFormulaItems property

Gets all items of power query formula.

```csharp
public PowerQueryFormulaItemCollection PowerQueryFormulaItems { get; }
```

### Examples

```csharp
// Called: item = workbook.DataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0];
public void PowerQueryFormula_Property_PowerQueryFormulaItems()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    PowerQueryFormulaItem item = workbook.DataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0];
    string str = item.Value.Replace(@"C:\", @"D:\");
    item.Value = str;
    workbook.Save(Constants.destPath + "example.xlsx");
    item = workbook.DataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0];
    Assert.AreEqual(str, item.Value);
}
```

### See Also

* class [PowerQueryFormulaItemCollection](../../powerqueryformulaitemcollection/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


