---
title: "WebExtensionBindingCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebExtensionBindingCollection. Obtient la relation de liaison d'extension web par l'index spécifique"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensionbindingcollection/item/
---
## WebExtensionBindingCollection indexer

Obtient la relation de liaison d'extension web par l'index spécifié.

```csharp
public WebExtensionBinding this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice. |

### Valeur de retour

La relation de liaison d'extension web

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une collection de liaisons d'extension web
            WebExtensionBindingCollection bindingCollection = new WebExtensionBindingCollection();

            // Ajouter une nouvelle liaison à la collection
            int index = bindingCollection.Add();

            // Accéder à la liaison en utilisant la propriété Item (lecture seule)
            WebExtensionBinding binding = bindingCollection[index];

            // Définir les propriétés de la liaison
            binding.Id = "binding1";
            binding.Type = "Text";
            binding.Appref = "Sheet1!A1";

            // Afficher les détails de la liaison
            Console.WriteLine("Binding ID: " + binding.Id);
            Console.WriteLine("Binding Type: " + binding.Type);
            Console.WriteLine("Binding AppRef: " + binding.Appref);

            // Modifier la liaison via la collection
            bindingCollection[index].Id = "modifiedBinding";
            Console.WriteLine("Modified Binding ID: " + bindingCollection[index].Id);

            // Enregistrez le classeur
            workbook.Save("WebExtensionBindingDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WebExtensionBinding](../../webextensionbinding/)
* class [WebExtensionBindingCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


