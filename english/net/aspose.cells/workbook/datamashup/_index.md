---
title: Workbook.DataMashup
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets mashup data
type: docs
url: /net/aspose.cells/workbook/datamashup/
---
## Workbook.DataMashup property

Gets mashup data.

```csharp
public DataMashup DataMashup { get; }
```

### Examples

```csharp
// Called: queries = workbook.DataMashup.PowerQueryFormulas;
public void Workbook_Property_DataMashup()
{
    var workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    var queries = workbook.DataMashup.PowerQueryFormulas;
    Assert.AreEqual(0x15, queries.Count);
    PowerQueryFormula formula = queries["Erreurs dans CLOTURE_FULL"];
    Assert.AreEqual(5, formula.PowerQueryFormulaItems.Count);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    queries = workbook.DataMashup.PowerQueryFormulas;
    Assert.AreEqual(0x15, queries.Count);
}
```

### See Also

* class [DataMashup](../../../aspose.cells.querytables/datamashup/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


