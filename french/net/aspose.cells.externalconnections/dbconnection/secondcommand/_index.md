---
title: "DBConnection.SecondCommand"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DBConnection. Spécifie une deuxième chaîne de texte de commande qui est conservée lorsque les champs de page basés sur le serveur de PivotTable sont utilisés. Pour les connexions ODBC, serverCommand est généralement une requête plus large que command, aucune clause WHERE n'étant présente dans la première. Sur la base de ces deux commandes Command et ServerCommand, l'interface utilisateur des paramètres peut être remplie et des requêtes paramétrées peuvent être construites"
type: docs
url: /fr/net/aspose.cells.externalconnections/dbconnection/secondcommand/
---
## DBConnection.SecondCommand property

Spécifie une deuxième chaîne de texte de commande qui est conservée lorsque les champs de page basés sur le serveur du tableau croisé dynamique sont utilisés. Pour les connexions ODBC, serverCommand est généralement une requête plus large que command (aucune clause WHERE n’est présente dans la première). En se basant sur ces 2 commandes (Command et ServerCommand), l’interface utilisateur des paramètres peut être remplie et des requêtes paramétrées peuvent être construites

```csharp
public override string SecondCommand { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertySecondCommandDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Créez une nouvelle instance DBConnection en l’ajoutant à la collection
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[0];
                
                // Configurer une connexion de base
                dbConnection.ConnectionString = "Server=myServer;Database=myDB;";
                dbConnection.CommandType = OLEDBCommandType.SqlStatement;
                dbConnection.Command = "SELECT * FROM Customers WHERE Country = 'USA'";
                
                // Définir et démontrer la propriété SecondCommand
                dbConnection.SecondCommand = "SELECT * FROM Customers";
                Console.WriteLine("SecondCommand value: " + dbConnection.SecondCommand);
                
                // Modifier le SecondCommand pour montrer qu’il est modifiable
                dbConnection.SecondCommand = "SELECT * FROM Orders";
                Console.WriteLine("Updated SecondCommand value: " + dbConnection.SecondCommand);
                
                // Enregistrez le classeur
                workbook.Save("SecondCommandDemo.xlsx");
                
                Console.WriteLine("SecondCommand demonstration completed successfully.");
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


