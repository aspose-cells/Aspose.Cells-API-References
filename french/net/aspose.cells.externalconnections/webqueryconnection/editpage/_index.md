---
title: "WebQueryConnection.EditPage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebQueryConnection. L'URL de la page Web destinée à l'utilisateur affichant les données de la requête Web. Cette URL est conservée dans le cas où sourceDatatrue et url ont été redirigés pour référencer un fichier XML. Ainsi, la page destinée à l'utilisateur peut être affichée dans l'interface et les données XML peuvent être récupérées en arrière-plan."
type: docs
url: /fr/net/aspose.cells.externalconnections/webqueryconnection/editpage/
---
## WebQueryConnection.EditPage property

L'URL de la page Web destinée à l'utilisateur affichant les données de la requête Web. Cette URL est conservée dans le cas où sourceData="true" et que l'url a été redirigée pour référencer un fichier XML. Ainsi, la page destinée à l'utilisateur peut être affichée dans l'interface, et les données XML peuvent être récupérées en arrière-plan.

```csharp
[Obsolete("Use WebQueryConnection.EditWebPage property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string EditPage { get; set; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété WebQueryConnection.EditWebPage. Cette propriété sera supprimée 12 mois plus tard depuis octobre 2017. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyEditPageDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Accédez à la première connexion de requête Web existante si disponible
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Afficher la valeur initiale de EditPage
                    Console.WriteLine("Initial EditPage value: " + connection.EditPage);
                    
                    // Définir EditPage à une nouvelle URL (car il est en lecture-écriture)
                    connection.EditPage = "https://example.com/editpage";
                    Console.WriteLine("Updated EditPage value: " + connection.EditPage);
                    
                    // Enregistrez le classeur
                    workbook.Save("WebQueryConnectionEditPageDemo.xlsx");
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


