---
title: PowerQueryFormulaFunction.F
second_title: Aspose.Cells for .NET API Reference
description: PowerQueryFormulaFunction property. Gets and sets the definition of function
type: docs
url: /net/aspose.cells.querytables/powerqueryformulafunction/f/
---
## PowerQueryFormulaFunction.F property

Gets and sets the definition of function.

```csharp
public string F { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;function (x as number) as datetimezone&amp;quot;, ((PowerQueryFormulaFunction)powerQueryFormula).F);        // HtmlSaveOptions
[Test]
        public void Property_F()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET572529.xlsx&quot;);
            var powerQueryFormula = workbook.DataMashup.PowerQueryFormulas[&quot;from_timestamp&quot;];
            Assert.AreEqual(&quot;from_timestamp&quot;, powerQueryFormula.Name);
            Assert.AreEqual(PowerQueryFormulaType.Function, powerQueryFormula.Type); // expected: Function, current value: Formula
            Assert.AreEqual(&quot;function (x as number) as datetimezone&quot;, ((PowerQueryFormulaFunction)powerQueryFormula).F);        // HtmlSaveOptions
            workbook.Save(Constants.destPath + &quot;CELLSNET572529.xlsx&quot;);
        }
```

### See Also

* class [PowerQueryFormulaFunction](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


