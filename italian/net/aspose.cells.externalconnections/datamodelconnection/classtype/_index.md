---
title: "DataModelConnection.ClassType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataModelConnection. Restituisce il tipo di questo oggetto ExternalConnection"
type: docs
url: /it/net/aspose.cells.externalconnections/datamodelconnection/classtype/
---
## DataModelConnection.ClassType property

Ottiene il tipo di questo [`ExternalConnection`](../../externalconnection/) oggetto.

```csharp
public override ExternalConnectionClassType ClassType { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Crea un'istanza di DataModelConnection utilizzando un oggetto non inizializzato
            DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
            ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

            // Visualizza il valore corrente di ClassType (proprietà di sola lettura)
            Console.WriteLine("Current ClassType value: " + connection.ClassType);

            // Imposta le proprietà di connessione
            connection.Command = "SELECT * FROM Products";
            connection.CommandType = OLEDBCommandType.SqlStatement;
            connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

            // Dimostra come ClassType influisce sulla gestione della connessione
            if (connection.ClassType == ExternalConnectionClassType.DataModel)
            {
                Console.WriteLine("This is a Data Model connection");
                // Aggiungi PowerQueryFormula per la connessione al modello di dati
                PowerQueryFormulaCollection queries = workbook.DataMashup.PowerQueryFormulas;
                string formulaDef = "let Source = Sql.Database(\"myServer\", \"myDB\") in Source";
                PowerQueryFormula query = (PowerQueryFormula)FormatterServices.GetUninitializedObject(typeof(PowerQueryFormula));
                query.Name = "ProductQuery";
                typeof(PowerQueryFormula).GetProperty("FormulaDefinition").SetValue(query, formulaDef);
                ((IList<PowerQueryFormula>)queries).Add(query);
            }

            // Salva la cartella di lavoro
            workbook.Save("DataModelConnectionClassTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


