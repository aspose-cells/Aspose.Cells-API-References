---
title: "ExternalConnection.SecondCommand"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Spécifie une chaîne de texte de deuxième commande qui est conservée lorsque les champs de page basés sur le serveur PivotTable sont utilisés. Pour les connexions ODBC, serverCommand est généralement une requête plus large que command, aucune clause WHERE n’est présente dans cette dernière. En fonction de ces 2 paramètres commandsCommand et ServerCommand, l’interface utilisateur des paramètres peut être remplie et des requêtes paramétrées peuvent être construites."
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/secondcommand/
---
## ExternalConnection.SecondCommand property

Spécifie une deuxième chaîne de texte de commande qui est conservée lorsque les champs de page basés sur le serveur du tableau croisé dynamique sont utilisés. Pour les connexions ODBC, serverCommand est généralement une requête plus large que command (aucune clause WHERE n’est présente dans la première). En se basant sur ces 2 commandes (Command et ServerCommand), l’interface utilisateur des paramètres peut être remplie et des requêtes paramétrées peuvent être construites

```csharp
public virtual string SecondCommand { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySecondCommandDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Accédez à la première connexion externe (en supposant qu’elle existe)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Afficher la valeur actuelle de SecondCommand (opération de lecture)
                Console.WriteLine("Initial SecondCommand value: " + connection.SecondCommand);
                
                // Définir une nouvelle valeur pour SecondCommand (puisqu’elle est en lecture‑écriture)
                connection.SecondCommand = "SELECT * FROM Customers WHERE Country = 'USA'";
                Console.WriteLine("Updated SecondCommand value: " + connection.SecondCommand);
                
                // Effacer SecondCommand pour démontrer la définition d’une chaîne vide
                connection.SecondCommand = string.Empty;
                Console.WriteLine("Cleared SecondCommand value: " + connection.SecondCommand);
                
                // Enregistrez le classeur avec les paramètres de connexion modifiés
                workbook.Save("SecondCommandDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


