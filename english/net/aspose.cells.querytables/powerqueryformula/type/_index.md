---
title: PowerQueryFormula.Type
second_title: Aspose.Cells for .NET API Reference
description: PowerQueryFormula property. Gets the type of this power query formula
type: docs
url: /net/aspose.cells.querytables/powerqueryformula/type/
---
## PowerQueryFormula.Type property

Gets the type of this power query formula.

```csharp
public virtual PowerQueryFormulaType Type { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(PowerQueryFormulaType.Function, queries[0].Type);
public void PowerQueryFormula_Property_Type()
{
    var workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    var queries = workbook.DataMashup.PowerQueryFormulas;
    Assert.AreEqual(1, queries.Count);
    Assert.AreEqual(PowerQueryFormulaType.Function, queries[0].Type);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


