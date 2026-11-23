---
title: "Classe SheetSet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Rendering.SheetSet. Décrit un ensemble de feuilles"
type: docs
url: /fr/net/aspose.cells.rendering/sheetset/
---
## SheetSet class

Décrit un ensemble de feuilles.

```csharp
public class SheetSet
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [SheetSet](sheetset/#constructor)(params int[]) | Crée un ensemble de feuilles basé sur les index de feuilles exacts. |
| [SheetSet](sheetset/#constructor_1)(params string[]) | Crée un ensemble de feuilles basé sur les noms de feuilles exacts. |

## Propriétés

| Nom | Description |
| --- | --- |
| static [Active](../../aspose.cells.rendering/sheetset/active/) { get; } | Obtient un ensemble avec la feuille active du classeur. |
| static [All](../../aspose.cells.rendering/sheetset/all/) { get; } | Obtient un ensemble avec toutes les feuilles du classeur dans leur ordre d'origine. |
| static [Visible](../../aspose.cells.rendering/sheetset/visible/) { get; } | Obtient un ensemble avec les feuilles visibles du classeur dans leur ordre d'origine. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetDemo
    {
        public static void SheetSetExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);   

            worksheet = workbook.Worksheets.Add("test1");
            worksheet.Cells["A1"].PutValue("test Data");
            worksheet.Cells["A2"].PutValue(234);
            worksheet.Cells["A3"].PutValue(333);
            worksheet.IsVisible = false;

            worksheet = workbook.Worksheets.Add("test2");
            worksheet.Cells["A1"].PutValue("test Data222");
            worksheet.Cells["A2"].PutValue(234444);
            worksheet.Cells["A3"].PutValue(333555);

            workbook.Worksheets.ActiveSheetIndex = 0;

            // Créez un objet PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Définissez la propriété SheetSet pour n'inclure que la feuille active
            pdfSaveOptions.SheetSet = SheetSet.Active;

            // Enregistrez le classeur dans un fichier PDF
            workbook.Save("SheetSetExample_ActiveSheet.pdf", pdfSaveOptions);

            // Définir la propriété SheetSet pour inclure toutes les feuilles visibles
            pdfSaveOptions.SheetSet = SheetSet.Visible;

            // Enregistrez le classeur dans un fichier PDF
            workbook.Save("SheetSetExample_VisibleSheets.pdf", pdfSaveOptions);

            // Définir la propriété SheetSet pour inclure toutes les feuilles
            pdfSaveOptions.SheetSet = SheetSet.All;

            // Enregistrez le classeur dans un fichier PDF
            workbook.Save("SheetSetExample_AllSheets.pdf", pdfSaveOptions);

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


