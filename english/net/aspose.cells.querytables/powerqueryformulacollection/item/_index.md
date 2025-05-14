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
// Called: dataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0].Value = dataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0].Value;
public void PowerQueryFormulaCollection_Property_Item()
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
// Called: var powerQueryFormula = workbook.DataMashup.PowerQueryFormulas["from_timestamp"];
public void PowerQueryFormulaCollection_Property_Item()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    var powerQueryFormula = workbook.DataMashup.PowerQueryFormulas["from_timestamp"];
    Assert.AreEqual("from_timestamp", powerQueryFormula.Name);
    Assert.AreEqual(PowerQueryFormulaType.Function, powerQueryFormula.Type); // expected: Function, current value: Formula
    Assert.AreEqual("function (x as number) as datetimezone", ((PowerQueryFormulaFunction)powerQueryFormula).F);        // HtmlSaveOptions
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


