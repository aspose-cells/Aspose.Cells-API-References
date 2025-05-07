---
title: DBConnection.PowerQueryFormula
second_title: Aspose.Cells for .NET API Reference
description: DBConnection property. Gets the definition of power query formula
type: docs
url: /net/aspose.cells.externalconnections/dbconnection/powerqueryformula/
---
## DBConnection.PowerQueryFormula property

Gets the definition of power query formula.

```csharp
public override PowerQueryFormula PowerQueryFormula { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(dbConn.PowerQueryFormula.FormulaDefinition == null);
[Test]
        public void Property_PowerQueryFormula()
        {

            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET47065.xlsx");
            ExternalConnectionCollection conns = workbook.DataConnections;
            foreach (ExternalConnection conn in conns)
            {
                DBConnection dbConn = conn as DBConnection;
                if (dbConn != null)
                {
                    Console.WriteLine(dbConn.ConnectionInfo);
                    Console.WriteLine(dbConn.PowerQueryFormula.FormulaDefinition);
                    Assert.IsFalse(dbConn.PowerQueryFormula.FormulaDefinition == null);
                }
            }
            workbook = new Workbook(Constants.sourcePath + "N47066.xlsm");
            conns = workbook.DataConnections;
            foreach (ExternalConnection conn in conns)
            {
                DBConnection dbConn = conn as DBConnection;
                if (dbConn != null)
                {
                    Console.WriteLine(dbConn.ConnectionInfo);
                    Console.WriteLine(dbConn.PowerQueryFormula.FormulaDefinition);
                    Assert.IsFalse(dbConn.PowerQueryFormula.FormulaDefinition == null);
                }
            }
        }
```

### See Also

* class [PowerQueryFormula](../../../aspose.cells.querytables/powerqueryformula/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


