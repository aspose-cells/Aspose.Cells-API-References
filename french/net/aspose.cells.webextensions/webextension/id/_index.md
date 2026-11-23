---
title: "WebExtension.Id"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebExtension. Obtient et définit l'identifiant unique de l'instance du module complémentaire Office dans le document actuel"
type: docs
url: /fr/net/aspose.cells.webextensions/webextension/id/
---
## WebExtension.Id property

Obtient et définit l'identifiant unique de l'instance Office Add-in dans le document actuel.

```csharp
public string Id { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyIdDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Obtenez la collection d'extensions web depuis le classeur
                var webExtensions = workbook.Worksheets.WebExtensions;
                
                // Ajoutez une nouvelle extension web (cela la créera avec les paramètres requis)
                int index = webExtensions.Add();
                WebExtension webExtension = webExtensions[index];
                
                // Définissez la propriété Id (puisqu'elle est en lecture-écriture)
                webExtension.Id = "SampleAddin123";
                
                // Affichez la valeur actuelle de la propriété Id
                Console.WriteLine($"WebExtension Id: {webExtension.Id}");
                
                // Modifiez la propriété Id pour démontrer qu'elle est modifiable
                webExtension.Id = "UpdatedAddin456";
                Console.WriteLine($"Updated WebExtension Id: {webExtension.Id}");
                
                // Enregistrez le classeur
                workbook.Save("WebExtensionIdDemo.xlsx");
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

* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


