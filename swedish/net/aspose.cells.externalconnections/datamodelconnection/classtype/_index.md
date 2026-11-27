---
title: "DataModelConnection.ClassType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataModelConnection‑egenskap. Hämtar typen av detta ExternalConnection‑objekt"
type: docs
url: /sv/net/aspose.cells.externalconnections/datamodelconnection/classtype/
---
## DataModelConnection.ClassType property

Hämtar typen av detta [`ExternalConnection`](../../externalconnection/)‑objekt.

```csharp
public override ExternalConnectionClassType ClassType { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.QueryTables;
    using System;
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Skapa en DataModelConnection‑instans med ett oinitierat objekt
            DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
            ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

            // Visa det aktuella ClassType‑värdet (skrivskyddad egenskap)
            Console.WriteLine("Current ClassType value: " + connection.ClassType);

            // Ställ in anslutningsegenskaper
            connection.Command = "SELECT * FROM Products";
            connection.CommandType = OLEDBCommandType.SqlStatement;
            connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

            // Demonstrera hur ClassType påverkar anslutningshantering
            if (connection.ClassType == ExternalConnectionClassType.DataModel)
            {
                Console.WriteLine("This is a Data Model connection");
                // Lägg till PowerQueryFormula för datamodellsanslutning
                PowerQueryFormulaCollection queries = workbook.DataMashup.PowerQueryFormulas;
                string formulaDef = "let Source = Sql.Database(\"myServer\", \"myDB\") in Source";
                PowerQueryFormula query = (PowerQueryFormula)FormatterServices.GetUninitializedObject(typeof(PowerQueryFormula));
                query.Name = "ProductQuery";
                typeof(PowerQueryFormula).GetProperty("FormulaDefinition").SetValue(query, formulaDef);
                ((IList<PowerQueryFormula>)queries).Add(query);
            }

            // Spara arbetsboken
            workbook.Save("DataModelConnectionClassTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


