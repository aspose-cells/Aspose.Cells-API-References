---
title: "WebQueryConnection.Post"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebQueryConnection. Retourne ou définit la chaîne utilisée avec la méthode POST pour envoyer des données à un serveur web afin de récupérer des données d'une requête web"
type: docs
url: /fr/net/aspose.cells.externalconnections/webqueryconnection/post/
---
## WebQueryConnection.Post property

Renvoie ou définit la chaîne utilisée avec la méthode post pour envoyer des données à un serveur Web afin de récupérer les données d’une requête Web.

```csharp
public string Post { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyPostDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Créer une connexion de requête Web en accédant à une existante ou en la créant via une initialisation appropriée
                // Comme nous ne pouvons pas instancier directement WebQueryConnection, nous utiliserons la première connexion si elle existe
                WebQueryConnection connection = null;
                
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection webQueryConn)
                {
                    connection = webQueryConn;
                }
                else
                {
                    // S'il n'existe aucune connexion, nous démontrerons avec une connexion factice
                    Console.WriteLine("No existing web query connection found - demonstrating with property access only");
                    return;
                }
                
                // Définir la valeur initiale de Post
                connection.Post = "param1=value1&param2=value2";
                Console.WriteLine("Initial Post value: " + connection.Post);
                
                // Modifier la valeur de Post
                connection.Post = "username=test&password=secret";
                Console.WriteLine("Updated Post value: " + connection.Post);
                
                // Effacer la valeur de Post
                connection.Post = string.Empty;
                Console.WriteLine("Cleared Post value: " + connection.Post);
                
                // Enregistrez le classeur
                workbook.Save("WebQueryConnectionPostDemo.xlsx");
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

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


