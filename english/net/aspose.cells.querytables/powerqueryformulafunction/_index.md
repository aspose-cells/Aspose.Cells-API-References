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
// Called: Assert.AreEqual(&amp;quot;function (x as number) as datetimezone&amp;quot;, ((PowerQueryFormulaFunction)powerQueryFormula).F);        // HtmlSaveOptions
[Test]
        public void Type_PowerQueryFormulaFunction()
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

* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


