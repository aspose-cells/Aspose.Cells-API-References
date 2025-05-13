---
title: Enum PowerQueryFormulaType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.QueryTables.PowerQueryFormulaType enum. Represents the type of power query formula
type: docs
url: /net/aspose.cells.querytables/powerqueryformulatype/
---
## PowerQueryFormulaType enumeration

Represents the type of power query formula.

```csharp
public enum PowerQueryFormulaType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Formula | `0` | Formula power query formula. |
| Function | `1` | Function power query formula. |
| Parameter | `2` | Parameter power query formula. |

### Examples

```csharp
// Called: Assert.AreEqual(PowerQueryFormulaType.Function, query3.Type);                      // NOT OK - expected PowerQueryFormulaType.Function
public void QueryTables_Type_PowerQueryFormulaType()
{
    var workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    var query1 = workbook.DataMashup.PowerQueryFormulas["Transform File (2)"];
   Assert.AreEqual(PowerQueryFormulaType.Function, query1.Type);                      // OK - PowerQueryFormulaType.Function
   Assert.AreEqual(1,query1.PowerQueryFormulaItems.Count); // OK - one item with key 'Source'

    var query2 = workbook.DataMashup.PowerQueryFormulas["fnSmartFolder"];
    Assert.AreEqual(PowerQueryFormulaType.Function, query2.Type);                      // NOT OK - expected PowerQueryFormulaType.Function
    Assert.AreEqual(1, query2.PowerQueryFormulaItems.Count);// NOT OK - expected one item with key 'fnSmartFolder' (or two items 'fn' and 'fnDocumentation')

    var query3 = workbook.DataMashup.PowerQueryFormulas["fnSmartFile"];
    Assert.AreEqual(PowerQueryFormulaType.Function, query3.Type);                      // NOT OK - expected PowerQueryFormulaType.Function
    Assert.AreEqual(1, query3.PowerQueryFormulaItems.Count); // NOT OK - expected one item with key 'fnSmartFile' (or two items 'fnSmartFile' and 'fnDocumentation')

    var query4 = workbook.DataMashup.PowerQueryFormulas["fnGetParameter"];
    Assert.AreEqual(PowerQueryFormulaType.Function, query4.Type);                      // NOT OK - expected PowerQueryFormulaType.Function
    Assert.AreEqual(1, query4.PowerQueryFormulaItems.Count);// NOT OK - expected one item with key 'fnGetParameter' (or two items 'fnGetParameter' and 'fnDocumentation')

    var query5 = workbook.DataMashup.PowerQueryFormulas["Transform File"];
    Assert.AreEqual(PowerQueryFormulaType.Function, query5.Type);                      // OK - PowerQueryFormulaType.Function
    Assert.AreEqual(1, query5.PowerQueryFormulaItems.Count); // OK - one item with key 'Source'
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


