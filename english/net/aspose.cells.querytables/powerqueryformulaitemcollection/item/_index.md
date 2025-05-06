---
title: PowerQueryFormulaItemCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: PowerQueryFormulaItemCollection property. Gets PowerQueryFormulaItem by the index in the list
type: docs
url: /net/aspose.cells.querytables/powerqueryformulaitemcollection/item/
---
## PowerQueryFormulaItemCollection indexer (1 of 2)

Gets [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) by the index in the list.

```csharp
public PowerQueryFormulaItem this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Examples

```csharp
// Called: PowerQueryFormulaItem item = workbook.DataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0];
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet47091.xlsx&quot;);
            PowerQueryFormulaItem item = workbook.DataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0];
            string str = item.Value.Replace(@&quot;C:\&quot;, @&quot;D:\&quot;);
            item.Value = str;
            workbook.Save(Constants.destPath + &quot;CellsNet47091.xlsx&quot;);
            item = workbook.DataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0];
            Assert.AreEqual(str, item.Value);
        }
```

### See Also

* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)

---

## PowerQueryFormulaItemCollection indexer (2 of 2)

Gets [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) by the name of the item.

```csharp
public PowerQueryFormulaItem this[string name] { get; }
```

| Parameter | Description |
| --- | --- |
| name | The name of the item. |

### See Also

* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


