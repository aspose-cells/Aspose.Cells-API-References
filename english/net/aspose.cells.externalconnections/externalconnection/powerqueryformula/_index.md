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
// Called: formula = connection.PowerQueryFormula;
[Test]
        public void Property_PowerQueryFormula()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET57031.xlsx");
            var connection = workbook.DataConnections[0];
            PowerQueryFormula formula = connection.PowerQueryFormula;
            Assert.AreEqual("end_time", formula.Name); // error: null, expected: end_time
            Assert.IsTrue(formula.FormulaDefinition != null); // error: null, expected: not null
            Assert.AreEqual(PowerQueryFormulaType.Parameter, formula.Type);
            Assert.AreEqual("1543392000", ((PowerQueryFormulaParameter)formula).Value);

            connection = workbook.DataConnections[1];
            formula = connection.PowerQueryFormula;

            Assert.AreEqual("fill_url", formula.Name); // error: null, expected: end_time
            Assert.IsTrue(formula.FormulaDefinition != null); // error: null, expected: not null


            connection = workbook.DataConnections[2];
            formula = connection.PowerQueryFormula;
            Assert.AreEqual("FIlls", formula.Name);
            Assert.IsTrue(formula.FormulaDefinition != null);
            workbook.Save(Constants.destPath + "CELLSNET57031.xlsx");

        }
```

### See Also

* class [PowerQueryFormula](../../../aspose.cells.querytables/powerqueryformula/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


