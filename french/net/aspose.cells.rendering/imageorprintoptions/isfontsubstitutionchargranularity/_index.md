---
title: "ImageOrPrintOptions.IsFontSubstitutionCharGranularity"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageOrPrintOptions. Indique s'il faut uniquement substituer la police du caractère lorsque la police de la cellule n'est pas compatible avec elle"
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/
---
## ImageOrPrintOptions.IsFontSubstitutionCharGranularity property

Indique s'il faut uniquement substituer la police du caractère lorsque la police de la cellule n'est pas compatible.

```csharp
public bool IsFontSubstitutionCharGranularity { get; set; }
```

### Remarques

La valeur par défaut est false. Nous essaierons d'abord la police par défaut du classeur et de PdfSaveOption/système pour la police de la cellule.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyIsFontSubstitutionCharGranularityDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Configurer la cellule avec une police potentiellement non prise en charge
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Text with unavailable font");
            Style style = cell.GetStyle();
            style.Font.Name = "NonExistentFont";
            cell.SetStyle(style);

            // Créer des options de rendu d'image
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Png, // Namespace reference now valid
                DefaultFont = "Arial",
                CheckWorkbookDefaultFont = false
            };

            // Afficher et modifier la valeur de la propriété
            Console.WriteLine($"Initial IsFontSubstitutionCharGranularity: {options.IsFontSubstitutionCharGranularity}");
            
            // Rendre avec le paramètre par défaut
            new SheetRender(worksheet, options).ToImage(0, "BeforeFontSubstitutionChange.png");

            // Modifier la propriété et rendre à nouveau
            options.IsFontSubstitutionCharGranularity = true;
            Console.WriteLine($"Updated IsFontSubstitutionCharGranularity: {options.IsFontSubstitutionCharGranularity}");
            new SheetRender(worksheet, options).ToImage(0, "AfterFontSubstitutionChange.png");

            // Enregistrer le classeur pour référence
            workbook.Save("FontSubstitutionDemoWorkbook.xlsx");
        }
    }
}
```

### Voir aussi

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


