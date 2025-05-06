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
// Called: Assert.AreEqual(x, dataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0].Value);
[Test]
        public void Property_PowerQueryFormulas()
        {
            Workbook excel = new Workbook(Constants.sourcePath + &quot;CELLSNET49145.xls&quot;);
            var dataMashup = excel.DataMashup;
            string x = &quot;Sql.Database(\&quot;SQL2K16\&quot;, \&quot;EUC876REG\&quot;, [Query=\&quot;select * from CANOTIFICATIONS\&quot;])&quot;;
            Assert.AreEqual(x, dataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0].Value);
            dataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0].Value = dataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0].Value;
            excel.Save(Constants.destPath + &quot;CELLSNET49145.xls&quot;);
            excel = new Workbook(Constants.destPath + &quot;CELLSNET49145.xls&quot;);
            Assert.AreEqual(x, dataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0].Value);
        }
```

### See Also

* class [PowerQueryFormulaCollection](../../powerqueryformulacollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


