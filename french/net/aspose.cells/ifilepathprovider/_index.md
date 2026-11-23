---
title: "Interface IFilePathProvider"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Interface Aspose.Cells.IFilePathProvider. Représente le fournisseur de chemin de fichier exporté"
type: docs
url: /fr/net/aspose.cells/ifilepathprovider/
---
## IFilePathProvider interface

Représente le fournisseur de chemin de fichier exporté.

```csharp
public interface IFilePathProvider
```

## Méthodes

| Nom | Description |
| --- | --- |
| [GetFullName](../../aspose.cells/ifilepathprovider/getfullname/)(string) | Obtient le chemin complet du fichier par le nom de la feuille de calcul lors de l'exportation de la feuille de calcul en HTML séparément. Ainsi, les références entre les feuilles de calcul peuvent être exportées correctement. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IFilePathProviderDemo : IFilePathProvider
    {
        // Implémentation de la méthode GetFullName de l'interface IFilePathProvider
        public string GetFullName(string sheetName)
        {
            // À des fins de démonstration, renvoie un chemin de fichier simple basé sur le nom de la feuille
            return $"{sheetName}.html";
        }

        public static void IFilePathProviderExample()
        {
            // Créer un nouveau classeur et ajouter des données
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Créer HtmlSaveOptions et définir le FilePathProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.FilePathProvider = new IFilePathProviderDemo();

            // Enregistrer le classeur au format HTML
            workbook.Save("IFilePathProviderExample.html", saveOptions);

            Console.WriteLine("Workbook saved to HTML with custom file paths.");
        }
    }


}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


