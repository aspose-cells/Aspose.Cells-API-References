---
title: "DataModelConnection.CommandType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataModelConnection‑egenskap. Returnerar OLEDBCommandType‑typen"
type: docs
url: /sv/net/aspose.cells.externalconnections/datamodelconnection/commandtype/
---
## DataModelConnection.CommandType property

Returnerar [`OLEDBCommandType`](../../oledbcommandtype/) typ.

```csharp
public override OLEDBCommandType CommandType { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.QueryTables;
    using System;
    using System.Collections.Generic;
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyCommandTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Skapa en DataModelConnection‑instans med ett oinitierat objekt
            DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
            ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);
            
            Console.WriteLine("Current CommandType value: " + connection.CommandType);

            connection.CommandType = OLEDBCommandType.SqlStatement;
            connection.Command = "SELECT * FROM Customers";
            connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

            PowerQueryFormulaCollection queries = workbook.DataMashup.PowerQueryFormulas;
            string formulaDef = "let Source = Sql.Database(\"myServer\", \"myDB\") in Source";
            // Skapa PowerQueryFormula med ett oinitierat objekt och ställ in egenskaper
            PowerQueryFormula query = (PowerQueryFormula)FormatterServices.GetUninitializedObject(typeof(PowerQueryFormula));
            query.Name = "SampleQuery";
            typeof(PowerQueryFormula).GetProperty("FormulaDefinition").SetValue(query, formulaDef);
            ((IList<PowerQueryFormula>)queries).Add(query);

            workbook.Save("PropertyCommandTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


