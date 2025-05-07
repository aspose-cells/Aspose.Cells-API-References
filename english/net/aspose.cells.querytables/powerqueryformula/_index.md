---
title: Class PowerQueryFormula
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.QueryTables.PowerQueryFormula class. Represents the definition of power query formula
type: docs
url: /net/aspose.cells.querytables/powerqueryformula/
---
## PowerQueryFormula class

Represents the definition of power query formula.

```csharp
public class PowerQueryFormula
```

## Properties

| Name | Description |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Gets and sets the description of the power query formula. |
| virtual [FormulaDefinition](../../aspose.cells.querytables/powerqueryformula/formuladefinition/) { get; } | Gets the definition of the power query formula. |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Gets the name of group which contains this power query formula. |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Gets and sets the name of the power query formula. |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Gets all items of power query formula. |
| virtual [Type](../../aspose.cells.querytables/powerqueryformula/type/) { get; } | Gets the type of this power query formula. |

### Examples

```csharp
// Called: PowerQueryFormula formula = connection.PowerQueryFormula;
[Test]
        public void Type_PowerQueryFormula()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET47649.xlsx");
            var connection = workbook.DataConnections[0];
            PowerQueryFormula formula = connection.PowerQueryFormula;
            Assert.AreEqual("AnwenderName", formula.Name); // error: null, expected: end_time
            Assert.IsTrue(formula.FormulaDefinition != null); // error: null, expected: not null


            connection = workbook.DataConnections[1];
            formula = connection.PowerQueryFormula;

            Assert.AreEqual("ApproxPauseFun", formula.Name); // error: null, expected: end_time
            Assert.IsTrue(formula.FormulaDefinition != null); // error: null, expected: not null
            workbook.Save(Constants.destPath + "CELLSNET47649.xlsx");

        }
```

### See Also

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


