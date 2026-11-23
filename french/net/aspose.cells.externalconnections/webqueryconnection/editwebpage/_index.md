---
title: "WebQueryConnection.EditWebPage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebQueryConnection. L'URL de la page Web destinée à l'utilisateur affichant les données de la requête Web. Cette URL est conservée dans le cas où sourceDatatrue et url ont été redirigés pour référencer un fichier XML. Ainsi, la page destinée à l'utilisateur peut être affichée dans l'interface et les données XML peuvent être récupérées en arrière-plan."
type: docs
url: /fr/net/aspose.cells.externalconnections/webqueryconnection/editwebpage/
---
## WebQueryConnection.EditWebPage property

L'URL de la page Web destinée à l'utilisateur affichant les données de la requête Web. Cette URL est conservée dans le cas où sourceData="true" et que l'url a été redirigée pour référencer un fichier XML. Ainsi, la page destinée à l'utilisateur peut être affichée dans l'interface, et les données XML peuvent être récupérées en arrière-plan.

```csharp
public string EditWebPage { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyEditWebPageDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Accéder à la première connexion de requête Web existante (le cas échéant)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Définissez la valeur initiale de EditWebPage
                    connection.EditWebPage = "https://example.com/user-facing-page.html";
                    Console.WriteLine("Initial EditWebPage value: " + connection.EditWebPage);
                    
                    // Mettez à jour la valeur de EditWebPage
                    connection.EditWebPage = "https://example.com/updated-user-page.html";
                    Console.WriteLine("Updated EditWebPage value: " + connection.EditWebPage);
                    
                    // Enregistrer le classeur avec la connexion de requête Web
                    workbook.Save("WebQueryConnectionEditWebPageDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connection found in the workbook.");
                }
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


