---
title: Enum PowerQueryFormulaType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.QueryTables.PowerQueryFormulaType enum. Represents the type of power query formula
type: docs
url: /net/aspose.cells.querytables/powerqueryformulatype/
---
## PowerQueryFormulaType enumeration

Represents the type of power query formula.

```csharp
public enum PowerQueryFormulaType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Formula | `0` | Formula power query formula. |
| Function | `1` | Function power query formula. |
| Parameter | `2` | Parameter power query formula. |

### Examples

```csharp
// Called: Assert.AreEqual(PowerQueryFormulaType.Function, powerQueryFormula.Type); // expected: Function, current value: Formula
[Test]
        public void Type_PowerQueryFormulaType()
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

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


