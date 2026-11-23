---
title: "WebExtension.AlterReferences"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebExtension. Obtient une liste de références alternatives"
type: docs
url: /fr/net/aspose.cells.webextensions/webextension/alterreferences/
---
## WebExtension.AlterReferences property

Obtient une liste de références alternatives.

```csharp
public WebExtensionReferenceCollection AlterReferences { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyAlterReferencesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Obtenez la collection d'extensions web depuis le classeur
                var webExtensions = workbook.Worksheets.WebExtensions;
                
                // Ajouter une nouvelle extension web
                int index = webExtensions.Add();
                WebExtension webExtension = webExtensions[index];
                
                // Accédez à la propriété AlterReferences (lecture seule)
                WebExtensionReferenceCollection alterReferences = webExtension.AlterReferences;
                
                // Afficher les informations sur les références d'altération
                Console.WriteLine($"Number of alter references: {alterReferences.Count}");
                
                // Ajouter une nouvelle référence d'altération (démontre l'utilisation de la collection)
                int newRefIndex = alterReferences.Add();
                Console.WriteLine($"Added new alter reference at index: {newRefIndex}");
                
                // Afficher le nombre mis à jour
                Console.WriteLine($"Updated number of alter references: {alterReferences.Count}");
                
                // Enregistrez le classeur
                workbook.Save("WebExtensionAlterReferencesDemo.xlsx");
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

* class [WebExtensionReferenceCollection](../../webextensionreferencecollection/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


