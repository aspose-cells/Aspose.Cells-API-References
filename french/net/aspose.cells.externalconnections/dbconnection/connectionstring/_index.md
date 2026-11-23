---
title: "DBConnection.ConnectionString"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DBConnection. La chaîne d’informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC"
type: docs
url: /fr/net/aspose.cells.externalconnections/dbconnection/connectionstring/
---
## DBConnection.ConnectionString property

La chaîne d’informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC.

```csharp
public override string ConnectionString { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyConnectionStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            try
            {
                // Accéder à la collection de connexions externes
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Créer une nouvelle DBConnection en l’ajoutant à la collection
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // Afficher la valeur initiale de ConnectionString
                Console.WriteLine("Initial ConnectionString: " + dbConnection.ConnectionString);

                // Définir une nouvelle chaîne de connexion
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";

                // Afficher la valeur mise à jour de ConnectionString
                Console.WriteLine("Updated ConnectionString: " + dbConnection.ConnectionString);

                // Enregistrez le classeur
                workbook.Save("ConnectionStringDemo.xlsx");
                Console.WriteLine("ConnectionString demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


