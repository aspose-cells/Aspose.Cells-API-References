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
// Called: Assert.AreEqual(PowerQueryFormulaType.Function, query2.Type);                      // NOT OK - expected PowerQueryFormulaType.Function
[Test]
        public void Type_PowerQueryFormulaType()
        {
            var workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET57739.xlsx&quot;);

            var query1 = workbook.DataMashup.PowerQueryFormulas[&quot;Transform File (2)&quot;];
           Assert.AreEqual(PowerQueryFormulaType.Function, query1.Type);                      // OK - PowerQueryFormulaType.Function
           Assert.AreEqual(1,query1.PowerQueryFormulaItems.Count); // OK - one item with key &apos;Source&apos;

            var query2 = workbook.DataMashup.PowerQueryFormulas[&quot;fnSmartFolder&quot;];
            Assert.AreEqual(PowerQueryFormulaType.Function, query2.Type);                      // NOT OK - expected PowerQueryFormulaType.Function
            Assert.AreEqual(1, query2.PowerQueryFormulaItems.Count);// NOT OK - expected one item with key &apos;fnSmartFolder&apos; (or two items &apos;fn&apos; and &apos;fnDocumentation&apos;)

            var query3 = workbook.DataMashup.PowerQueryFormulas[&quot;fnSmartFile&quot;];
            Assert.AreEqual(PowerQueryFormulaType.Function, query3.Type);                      // NOT OK - expected PowerQueryFormulaType.Function
            Assert.AreEqual(1, query3.PowerQueryFormulaItems.Count); // NOT OK - expected one item with key &apos;fnSmartFile&apos; (or two items &apos;fnSmartFile&apos; and &apos;fnDocumentation&apos;)

            var query4 = workbook.DataMashup.PowerQueryFormulas[&quot;fnGetParameter&quot;];
            Assert.AreEqual(PowerQueryFormulaType.Function, query4.Type);                      // NOT OK - expected PowerQueryFormulaType.Function
            Assert.AreEqual(1, query4.PowerQueryFormulaItems.Count);// NOT OK - expected one item with key &apos;fnGetParameter&apos; (or two items &apos;fnGetParameter&apos; and &apos;fnDocumentation&apos;)

            var query5 = workbook.DataMashup.PowerQueryFormulas[&quot;Transform File&quot;];
            Assert.AreEqual(PowerQueryFormulaType.Function, query5.Type);                      // OK - PowerQueryFormulaType.Function
            Assert.AreEqual(1, query5.PowerQueryFormulaItems.Count); // OK - one item with key &apos;Source&apos;
            workbook.Save(Constants.destPath + &quot;CELLSNET57739.xlsx&quot;);
        }
```

### See Also

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


