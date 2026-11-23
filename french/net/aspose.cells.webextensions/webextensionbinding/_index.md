---
title: "Classe WebExtensionBinding"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.WebExtensions.WebExtensionBinding. Représente une relation de liaison entre un module complémentaire Office et les données du document"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensionbinding/
---
## WebExtensionBinding class

Représente une relation de liaison entre un Office Add-in et les données du document.

```csharp
public class WebExtensionBinding
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [WebExtensionBinding](webextensionbinding/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Appref](../../aspose.cells.webextensions/webextensionbinding/appref/) { get; set; } | Obtient et définit la clé de liaison utilisée pour associer l'entrée de liaison dans cette liste aux données liées dans le document. |
| [Id](../../aspose.cells.webextensions/webextensionbinding/id/) { get; set; } | Obtient et définit l'identifiant de liaison. |
| [Type](../../aspose.cells.webextensions/webextensionbinding/type/) { get; set; } | Obtient et définit le type de liaison. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionBindingDemo
    {
        public static void Run()
        {
            try
            {
                // Créer une nouvelle instance de WebExtensionBinding
                WebExtensionBinding binding = new WebExtensionBinding();

                // Définir les propriétés
                binding.Id = "DemoBinding";
                binding.Type = "range";
                binding.Appref = "Sheet1!A1";

                // Afficher les valeurs des propriétés
                Console.WriteLine($"Binding created - ID: {binding.Id}, Type: {binding.Type}, Appref: {binding.Appref}");

                // Modifier les propriétés
                binding.Appref = "Sheet1!B2";
                Console.WriteLine($"Updated Appref: {binding.Appref}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebExtensionBinding: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


