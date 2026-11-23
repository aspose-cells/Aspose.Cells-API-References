---
title: "DBConnection.CommandType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DBConnection. Spécifie le type de commande OLE DB. 1. La requête spécifie un nom de cube 2. La requête spécifie une instruction SQL 3. La requête spécifie un nom de table 4. La requête indique que des informations par défaut ont été fournies et qu’il appartient au fournisseur de les interpréter 5. La requête porte sur un fournisseur de données de liste basé sur le web"
type: docs
url: /fr/net/aspose.cells.externalconnections/dbconnection/commandtype/
---
## DBConnection.CommandType property

Spécifie le type de commande OLE DB. 1. Query spécifie un nom de cube 2. Query spécifie une instruction SQL 3. Query spécifie un nom de table 4. Query spécifie que des informations par défaut ont été fournies, et il revient au fournisseur de les interpréter. 5. Query porte sur un fournisseur de données de liste basé sur le web.

```csharp
public override OLEDBCommandType CommandType { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;

    public class DBConnectionPropertyCommandTypeDemo
    {
        public static void Run()
        {
            // Initialiser un classeur (vide ou à partir d'un fichier pouvant contenir des connexions)
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
                    // Afficher la valeur actuelle de CommandType
                    Console.WriteLine("Original CommandType: " + dbConn.CommandType);

                    // Démontrer la définition de CommandType (propriété lecture‑écriture)
                    dbConn.CommandType = OLEDBCommandType.SqlStatement;
                    Console.WriteLine("Updated CommandType: " + dbConn.CommandType);
                }

                // Enregistrer le classeur (même s'il n'est pas modifié) pour illustrer un flux complet)
                workbook.Save("CommandTypeDemo.xlsx");
                Console.WriteLine("Workbook saved as CommandTypeDemo.xlsx");
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

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


