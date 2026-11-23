---
title: "WebExtensionPropertyCollection.RemoveAt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WebExtensionPropertyCollection. Supprime la propriété par son nom"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensionpropertycollection/removeat/
---
## WebExtensionPropertyCollection.RemoveAt method

Supprime la propriété par son nom.

```csharp
public void RemoveAt(string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de la propriété. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyCollectionMethodRemoveAtWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une collection de propriétés d'extension web
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // Ajouter quelques propriétés à la collection
            properties.Add("Property1", "Value1");
            properties.Add("Property2", "Value2");
            properties.Add("Property3", "Value3");

            try
            {
                // Appeler la méthode RemoveAt avec un paramètre string
                properties.RemoveAt("Property2");

                Console.WriteLine("Property with name 'Property2' removed successfully.");
                
                // Afficher les propriétés restantes
                Console.WriteLine("Remaining properties:");
                for (int i = 0; i < properties.Count; i++)
                {
                    Console.WriteLine($"{properties[i].Name}: {properties[i].Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("WebExtensionPropertyCollectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


