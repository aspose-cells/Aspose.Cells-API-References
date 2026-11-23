---
title: "DataModelConnection.CommandType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataModelConnection. Retourne le type OLEDBCommandType"
type: docs
url: /fr/net/aspose.cells.externalconnections/datamodelconnection/commandtype/
---
## DataModelConnection.CommandType property

Retourne le type [`OLEDBCommandType`](../../oledbcommandtype/).

```csharp
public override OLEDBCommandType CommandType { get; set; }
```

### Exemples

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
            
            // Créer une instance de DataModelConnection en utilisant un objet non initialisé
            DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
            ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);
            
            Console.WriteLine("Current CommandType value: " + connection.CommandType);

            connection.CommandType = OLEDBCommandType.SqlStatement;
            connection.Command = "SELECT * FROM Customers";
            connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

            PowerQueryFormulaCollection queries = workbook.DataMashup.PowerQueryFormulas;
            string formulaDef = "let Source = Sql.Database(\"myServer\", \"myDB\") in Source";
            // Créer PowerQueryFormula en utilisant un objet non initialisé et définir les propriétés
            PowerQueryFormula query = (PowerQueryFormula)FormatterServices.GetUninitializedObject(typeof(PowerQueryFormula));
            query.Name = "SampleQuery";
            typeof(PowerQueryFormula).GetProperty("FormulaDefinition").SetValue(query, formulaDef);
            ((IList<PowerQueryFormula>)queries).Add(query);

            workbook.Save("PropertyCommandTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


