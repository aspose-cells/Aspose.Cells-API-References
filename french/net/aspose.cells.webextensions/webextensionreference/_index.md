---
title: "Classe WebExtensionReference"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.WebExtensions.WebExtensionReference. Représente l’identification de l’emplacement du fournisseur et de la version de l’extension"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensionreference/
---
## WebExtensionReference class

Représente l'identification de l'emplacement du fournisseur et de la version de l'extension.

```csharp
public class WebExtensionReference
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Id](../../aspose.cells.webextensions/webextensionreference/id/) { get; set; } | Obtient et définit l’identifiant associé à l’Office Add‑in au sein d’un fournisseur de catalogue. L’identifiant DOIT être unique au sein d’un fournisseur de catalogue. |
| [StoreName](../../aspose.cells.webextensions/webextensionreference/storename/) { get; set; } | Obtient et définit l’instance du marketplace où l’Office Add‑in est stocké. |
| [StoreType](../../aspose.cells.webextensions/webextensionreference/storetype/) { get; set; } | Obtient et définit le type de marketplace que l’attribut de magasin identifie. |
| [Version](../../aspose.cells.webextensions/webextensionreference/version/) { get; set; } | Obtient et définit la version. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionReferenceDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Créez d’abord une WebExtension
                WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
                int extensionIndex = webExtensions.Add();
                WebExtension webExt = webExtensions[extensionIndex];

                // Obtenez le WebExtensionReference à partir de la WebExtension
                WebExtensionReference webExtensionRef = webExt.Reference;

                // Définissez les propriétés du WebExtensionReference
                webExtensionRef.Id = "my-addin-123";
                webExtensionRef.Version = "1.0.0";
                webExtensionRef.StoreName = "MyAddinStore";
                webExtensionRef.StoreType = WebExtensionStoreType.OMEX;

                // Affichez les propriétés de référence
                Console.WriteLine($"WebExtension Reference created:");
                Console.WriteLine($"ID: {webExtensionRef.Id}");
                Console.WriteLine($"Version: {webExtensionRef.Version}");
                Console.WriteLine($"Store Name: {webExtensionRef.StoreName}");
                Console.WriteLine($"Store Type: {webExtensionRef.StoreType}");

                // Enregistrez le classeur
                workbook.Save("WebExtensionReferenceDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with WebExtension reference.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebExtensionReference: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


