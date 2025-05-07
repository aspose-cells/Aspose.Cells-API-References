---
title: Class PowerQueryFormulaFunction
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.QueryTables.PowerQueryFormulaFunction class. Represents the function of power query
type: docs
url: /net/aspose.cells.querytables/powerqueryformulafunction/
---
## PowerQueryFormulaFunction class

Represents the function of power query.

```csharp
public class PowerQueryFormulaFunction : PowerQueryFormula
```

## Properties

| Name | Description |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Gets and sets the description of the power query formula.(Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| [F](../../aspose.cells.querytables/powerqueryformulafunction/f/) { get; set; } | Gets and sets the definition of function. |
| virtual [FormulaDefinition](../../aspose.cells.querytables/powerqueryformula/formuladefinition/) { get; } | Gets the definition of the power query formula.(Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Gets the name of group which contains this power query formula.(Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Gets and sets the name of the power query formula.(Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Gets all items of power query formula.(Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| override [Type](../../aspose.cells.querytables/powerqueryformulafunction/type/) { get; } | Gets the type of power query formula. |

### Examples

```csharp
// Called: Assert.AreEqual("function (x as number) as datetimezone", ((PowerQueryFormulaFunction)powerQueryFormula).F);        // HtmlSaveOptions
[Test]
        public void Type_PowerQueryFormulaFunction()
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

* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


