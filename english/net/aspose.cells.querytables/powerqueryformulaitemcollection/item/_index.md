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
// Called: Assert.AreEqual(x, dataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0].Value);
public void PowerQueryFormulaItemCollection_Property_Item()
{
    Workbook excel = new Workbook(Constants.sourcePath + "example.xls");
    var dataMashup = excel.DataMashup;
    string x = "Sql.Database(\"SQL2K16\", \"EUC876REG\", [Query=\"select * from CANOTIFICATIONS\"])";
    Assert.AreEqual(x, dataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0].Value);
    dataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0].Value = dataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0].Value;
    excel.Save(Constants.destPath + "example.xls");
    excel = new Workbook(Constants.destPath + "example.xls");
    Assert.AreEqual(x, dataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0].Value);
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


