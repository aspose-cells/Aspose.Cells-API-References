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
// Called: item = workbook.DataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0];
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet47091.xlsx");
            PowerQueryFormulaItem item = workbook.DataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0];
            string str = item.Value.Replace(@"C:\", @"D:\");
            item.Value = str;
            workbook.Save(Constants.destPath + "CellsNet47091.xlsx");
            item = workbook.DataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0];
            Assert.AreEqual(str, item.Value);
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
// Called: f = mashupData.PowerQueryFormulas["Sample File"];
[Test]
        public void Property_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet53328.xlsx");
            Aspose.Cells.QueryTables.DataMashup mashupData = workbook.DataMashup;

            Aspose.Cells.QueryTables.PowerQueryFormula f = mashupData.PowerQueryFormulas["Transform File"];
            Assert.AreEqual(PowerQueryFormulaType.Function, f.Type);
            Assert.IsTrue(f.FormulaDefinition.IndexOf("in") != -1);

            f = mashupData.PowerQueryFormulas["Sample File"];
            Assert.AreEqual(3, f.PowerQueryFormulaItems.Count);
            Assert.IsTrue(f.PowerQueryFormulaItems[2].Value.IndexOf("[ FunctionQueryBinding") == -1);
            workbook.Save(Constants.destPath + "CellsNet53328.xlsx");
        }
```

### See Also

* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


