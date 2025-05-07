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
// Called: Assert.AreEqual("function (x as number) as datetimezone", ((PowerQueryFormulaFunction)powerQueryFormula).F);        // HtmlSaveOptions
[Test]
        public void Property_F()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET572529.xlsx");
            var powerQueryFormula = workbook.DataMashup.PowerQueryFormulas["from_timestamp"];
            Assert.AreEqual("from_timestamp", powerQueryFormula.Name);
            Assert.AreEqual(PowerQueryFormulaType.Function, powerQueryFormula.Type); // expected: Function, current value: Formula
            Assert.AreEqual("function (x as number) as datetimezone", ((PowerQueryFormulaFunction)powerQueryFormula).F);        // HtmlSaveOptions
            workbook.Save(Constants.destPath + "CELLSNET572529.xlsx");
        }
```

### See Also

* class [PowerQueryFormulaFunction](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


