---
title: "DataModelConnection.ClassType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataModelConnection-Eigenschaft. Gibt den Typ dieses ExternalConnection-Objekts zurück"
type: docs
url: /de/net/aspose.cells.externalconnections/datamodelconnection/classtype/
---
## DataModelConnection.ClassType property

Gibt den Typ dieses [`ExternalConnection`](../../externalconnection/) Objekts zurück.

```csharp
public override ExternalConnectionClassType ClassType { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Erstellen Sie eine DataModelConnection-Instanz mit einem nicht initialisierten Objekt
            DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
            ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

            // Zeigen Sie den aktuellen ClassType-Wert an (schreibgeschützte Eigenschaft)
            Console.WriteLine("Current ClassType value: " + connection.ClassType);

            // Richten Sie Verbindungseigenschaften ein
            connection.Command = "SELECT * FROM Products";
            connection.CommandType = OLEDBCommandType.SqlStatement;
            connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

            // Demonstrieren Sie, wie der ClassType die Verbindungsbehandlung beeinflusst
            if (connection.ClassType == ExternalConnectionClassType.DataModel)
            {
                Console.WriteLine("This is a Data Model connection");
                // PowerQueryFormula zur Datenmodellverbindung hinzufügen
                PowerQueryFormulaCollection queries = workbook.DataMashup.PowerQueryFormulas;
                string formulaDef = "let Source = Sql.Database(\"myServer\", \"myDB\") in Source";
                PowerQueryFormula query = (PowerQueryFormula)FormatterServices.GetUninitializedObject(typeof(PowerQueryFormula));
                query.Name = "ProductQuery";
                typeof(PowerQueryFormula).GetProperty("FormulaDefinition").SetValue(query, formulaDef);
                ((IList<PowerQueryFormula>)queries).Add(query);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("DataModelConnectionClassTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


