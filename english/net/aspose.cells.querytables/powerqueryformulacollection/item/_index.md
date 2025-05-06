---
title: PowerQueryFormulaCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: PowerQueryFormulaCollection property. Gets PowerQueryFormula by the index in the list
type: docs
url: /net/aspose.cells.querytables/powerqueryformulacollection/item/
---
## PowerQueryFormulaCollection indexer (1 of 2)

Gets [`PowerQueryFormula`](../../powerqueryformula/) by the index in the list.

```csharp
public PowerQueryFormula this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Examples

```csharp
// Called: Assert.AreEqual(PowerQueryFormulaType.Function, queries[0].Type);
[Test]
        public void Property_Int32_()
        {
            var workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET57740.xlsx&quot;);
            var queries = workbook.DataMashup.PowerQueryFormulas;
            Assert.AreEqual(1, queries.Count);
            Assert.AreEqual(PowerQueryFormulaType.Function, queries[0].Type);
            workbook.Save(Constants.destPath + &quot;CELLSNET57740.xlsx&quot;);
        }
```

### See Also

* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)

---

## PowerQueryFormulaCollection indexer (2 of 2)

Gets [`PowerQueryFormula`](../../powerqueryformula/) by the name of the power query formula.

```csharp
public PowerQueryFormula this[string name] { get; }
```

| Parameter | Description |
| --- | --- |
| name | The name of the item. |

### Examples

```csharp
// Called: PowerQueryFormula formula = queries[&amp;quot;Erreurs dans CLOTURE_FULL&amp;quot;];
[Test]
        public void Property_String_()
        {
            var workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET58132.xlsx&quot;);
            var queries = workbook.DataMashup.PowerQueryFormulas;
            Assert.AreEqual(0x15, queries.Count);
            PowerQueryFormula formula = queries[&quot;Erreurs dans CLOTURE_FULL&quot;];
            Assert.AreEqual(5, formula.PowerQueryFormulaItems.Count);
            workbook.Save(Constants.destPath + &quot;CELLSNET58132.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET58132.xlsx&quot;);
            queries = workbook.DataMashup.PowerQueryFormulas;
            Assert.AreEqual(0x15, queries.Count);
        }
```

### See Also

* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


