---
title: "DataModelConnection.CommandType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataModelConnection-Eigenschaft. Gibt den Typ OLEDBCommandType zurück"
type: docs
url: /de/net/aspose.cells.externalconnections/datamodelconnection/commandtype/
---
## DataModelConnection.CommandType property

Gibt den Typ [`OLEDBCommandType`](../../oledbcommandtype/) zurück.

```csharp
public override OLEDBCommandType CommandType { get; set; }
```

### Beispiele

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
            
            // Erstellen Sie eine DataModelConnection-Instanz mit einem nicht initialisierten Objekt
            DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
            ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);
            
            Console.WriteLine("Current CommandType value: " + connection.CommandType);

            connection.CommandType = OLEDBCommandType.SqlStatement;
            connection.Command = "SELECT * FROM Customers";
            connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

            PowerQueryFormulaCollection queries = workbook.DataMashup.PowerQueryFormulas;
            string formulaDef = "let Source = Sql.Database(\"myServer\", \"myDB\") in Source";
            // PowerQueryFormula mit nicht initialisiertem Objekt erstellen und Eigenschaften festlegen
            PowerQueryFormula query = (PowerQueryFormula)FormatterServices.GetUninitializedObject(typeof(PowerQueryFormula));
            query.Name = "SampleQuery";
            typeof(PowerQueryFormula).GetProperty("FormulaDefinition").SetValue(query, formulaDef);
            ((IList<PowerQueryFormula>)queries).Add(query);

            workbook.Save("PropertyCommandTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


