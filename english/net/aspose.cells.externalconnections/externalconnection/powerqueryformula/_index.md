---
title: ExternalConnection.PowerQueryFormula
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. Gets the definition of power query formula
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/powerqueryformula/
---
## ExternalConnection.PowerQueryFormula property

Gets the definition of power query formula.

```csharp
public virtual PowerQueryFormula PowerQueryFormula { get; }
```

### Examples

```csharp
// Called: PowerQueryFormula formula = connection.PowerQueryFormula;
[Test]
        public void Property_PowerQueryFormula()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET47649.xlsx&quot;);
            var connection = workbook.DataConnections[0];
            PowerQueryFormula formula = connection.PowerQueryFormula;
            Assert.AreEqual(&quot;AnwenderName&quot;, formula.Name); // error: null, expected: end_time
            Assert.IsTrue(formula.FormulaDefinition != null); // error: null, expected: not null


            connection = workbook.DataConnections[1];
            formula = connection.PowerQueryFormula;

            Assert.AreEqual(&quot;ApproxPauseFun&quot;, formula.Name); // error: null, expected: end_time
            Assert.IsTrue(formula.FormulaDefinition != null); // error: null, expected: not null
            workbook.Save(Constants.destPath + &quot;CELLSNET47649.xlsx&quot;);

        }
```

### See Also

* class [PowerQueryFormula](../../../aspose.cells.querytables/powerqueryformula/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


