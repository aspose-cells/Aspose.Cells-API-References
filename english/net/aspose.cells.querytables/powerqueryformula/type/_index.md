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
// Called: Assert.AreEqual(PowerQueryFormulaType.Function, f.Type);
[Test]
        public void Property_Type()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet53328.xlsx&quot;);
            Aspose.Cells.QueryTables.DataMashup mashupData = workbook.DataMashup;

            Aspose.Cells.QueryTables.PowerQueryFormula f = mashupData.PowerQueryFormulas[&quot;Transform File&quot;];
            Assert.AreEqual(PowerQueryFormulaType.Function, f.Type);
            Assert.IsTrue(f.FormulaDefinition.IndexOf(&quot;in&quot;) != -1);

            f = mashupData.PowerQueryFormulas[&quot;Sample File&quot;];
            Assert.AreEqual(3, f.PowerQueryFormulaItems.Count);
            Assert.IsTrue(f.PowerQueryFormulaItems[2].Value.IndexOf(&quot;[ FunctionQueryBinding&quot;) == -1);
            workbook.Save(Constants.destPath + &quot;CellsNet53328.xlsx&quot;);
        }
```

### See Also

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


