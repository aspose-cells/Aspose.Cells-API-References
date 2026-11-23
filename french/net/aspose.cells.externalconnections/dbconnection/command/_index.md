---
title: "DBConnection.Command"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DBConnection. La chaîne contenant la commande de base de données à transmettre à l'API du fournisseur de données qui interagira avec la source externe afin de récupérer les données"
type: docs
url: /fr/net/aspose.cells.externalconnections/dbconnection/command/
---
## DBConnection.Command property

La chaîne contenant la commande de base de données à transmettre à l’API du fournisseur de données qui interagira avec la source externe afin de récupérer les données

```csharp
public override string Command { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyCommandDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            try
            {
                // Accéder à la collection de connexions externes
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Trouver le premier DBConnection dans la collection (le cas échéant)
                DBConnection dbConn = null;
                foreach (ExternalConnection conn in connections)
                {
                    if (conn is DBConnection dbConnection)
                    {
                        dbConn = dbConnection;
                        break;
                    }
                }

                if (dbConn == null)
                {
                    Console.WriteLine("No DBConnection objects found in the workbook.");
                }
                else
                {
                    // Afficher la valeur actuelle de Command (opération de lecture)
                    Console.WriteLine("Current Command: " + dbConn.Command);

                    // Démontrer la définition de Command (propriété lecture‑écriture)
                    dbConn.Command = "SELECT * FROM Customers";
                    Console.WriteLine("Updated Command: " + dbConn.Command);
                }

                // Enregistrez le classeur
                workbook.Save("CommandDemo.xlsx");
                Console.WriteLine("Workbook saved as CommandDemo.xlsx");
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


