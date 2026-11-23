---
title: "DBConnection.ConnectionInfo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DBConnection. La chaîne d’informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC"
type: docs
url: /fr/net/aspose.cells.externalconnections/dbconnection/connectioninfo/
---
## DBConnection.ConnectionInfo property

La chaîne d’informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC.

```csharp
[Obsolete("Use ExternalConnection.ConnectionString property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string ConnectionInfo { get; set; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété ExternalConnection.ConnectionString. Cette méthode sera supprimée 12 mois plus tard, depuis octobre 2024. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyConnectionInfoDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            try
            {
                // Créez une nouvelle instance DBConnection en l’ajoutant à la collection
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // Configurer une connexion de base pour démontrer la propriété ConnectionInfo
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";

                // Afficher la valeur actuelle de la propriété ConnectionInfo
                Console.WriteLine("Current ConnectionInfo value: " + dbConnection.ConnectionInfo);

                // Étant donné que ConnectionInfo n’est pas en lecture seule, démontrer sa définition
                dbConnection.ConnectionInfo = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=D:\\data\\database.mdb;";
                Console.WriteLine("Updated ConnectionInfo value: " + dbConnection.ConnectionInfo);

                // Enregistrez le classeur
                workbook.Save("ConnectionInfoDemo.xlsx");

                Console.WriteLine("ConnectionInfo demonstration completed successfully.");
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


