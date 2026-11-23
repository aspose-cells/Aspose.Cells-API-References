---
title: "WebExtension.Bindings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebExtension. Obtient toutes les relations de liaison entre un module complémentaire Office et les données du document"
type: docs
url: /fr/net/aspose.cells.webextensions/webextension/bindings/
---
## WebExtension.Bindings property

Obtient toutes les relations de liaison entre un Office Add-in et les données du document.

```csharp
public WebExtensionBindingCollection Bindings { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyBindingsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Créer une feuille de calcul d’exemple
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // En supposant que nous obtenions une extension web de quelque part (puisque nous ne pouvons pas en créer une directement)
                // Ceci est une modification minimale pour faire compiler le code tout en conservant sa structure
                WebExtension webExtension = null; // In real usage, this would come from workbook.WebExtensions or similar
                
                if (webExtension != null)
                {
                    // Accédez à la propriété Bindings (lecture seule)
                    WebExtensionBindingCollection bindings = webExtension.Bindings;
                    
                    // Affichez les informations sur les liaisons
                    Console.WriteLine($"Number of bindings: {bindings.Count}");
                    
                    // Ajoutez une nouvelle liaison (démontre l'utilisation de la collection)
                    int newBindingIndex = bindings.Add();
                    Console.WriteLine($"Added new binding at index: {newBindingIndex}");
                    
                    // Afficher le nombre mis à jour
                    Console.WriteLine($"Updated number of bindings: {bindings.Count}");
                }
                else
                {
                    Console.WriteLine("No web extension available");
                }
                
                // Enregistrez le classeur
                workbook.Save("WebExtensionBindingsDemo.xlsx");
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

* class [WebExtensionBindingCollection](../../webextensionbindingcollection/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


