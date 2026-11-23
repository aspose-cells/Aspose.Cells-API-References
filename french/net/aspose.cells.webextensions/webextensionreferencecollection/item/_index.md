---
title: "WebExtensionReferenceCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebExtensionReferenceCollection. Obtient l'extension web par l'index spécifique"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensionreferencecollection/item/
---
## WebExtensionReferenceCollection indexer

Obtient l'extension web par l'index spécifique.

```csharp
public WebExtensionReference this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice. |

### Valeur de retour

L'extension web

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionReferenceCollectionPropertyItemDemo
    {
        public static void Run()
        {
            try
            {
                // Créer une nouvelle WebExtensionReferenceCollection
                WebExtensionReferenceCollection references = new WebExtensionReferenceCollection();
                
                // Ajoute une nouvelle référence d'extension web
                int index = references.Add();
                
                // Accéder à la propriété Item (lecture seule) pour obtenir la référence à l'index spécifié
                WebExtensionReference reference = references[index];
                
                // Afficher les informations sur la référence récupérée
                Console.WriteLine($"Retrieved web extension reference at index: {index}");
                Console.WriteLine($"Reference type: {reference.GetType().Name}");
                
                // Remarque : la propriété Item est en lecture seule, nous ne faisons donc que démontrer la récupération de sa valeur
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating Item property: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [WebExtensionReference](../../webextensionreference/)
* class [WebExtensionReferenceCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


