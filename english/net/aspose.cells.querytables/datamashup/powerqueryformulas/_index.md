---
title: DataMashup.PowerQueryFormulas
second_title: Aspose.Cells for .NET API Reference
description: DataMashup property. Gets all power query formulas
type: docs
url: /net/aspose.cells.querytables/datamashup/powerqueryformulas/
---
## DataMashup.PowerQueryFormulas property

Gets all power query formulas.

```csharp
public PowerQueryFormulaCollection PowerQueryFormulas { get; }
```

### Examples

```csharp
// Called: dataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0].Value = dataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0].Value;
[Test]
        public void Property_PowerQueryFormulas()
        {
            Workbook excel = new Workbook(Constants.sourcePath + "CELLSNET49145.xls");
            var dataMashup = excel.DataMashup;
            string x = "Sql.Database(\"SQL2K16\", \"EUC876REG\", [Query=\"select * from CANOTIFICATIONS\"])";
            Assert.AreEqual(x, dataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0].Value);
            dataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0].Value = dataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0].Value;
            excel.Save(Constants.destPath + "CELLSNET49145.xls");
            excel = new Workbook(Constants.destPath + "CELLSNET49145.xls");
            Assert.AreEqual(x, dataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0].Value);
        }
```

### See Also

* class [PowerQueryFormulaCollection](../../powerqueryformulacollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


