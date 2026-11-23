---
title: "ImageOrPrintOptions.IsCellAutoFit"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageOrPrintOptions. Indique si la largeur et la hauteur des cellules sont automatiquement ajustées en fonction de la valeur de la cellule. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/iscellautofit/
---
## ImageOrPrintOptions.IsCellAutoFit property

Indique si la largeur et la hauteur des cellules sont automatiquement ajustées en fonction de la valeur de la cellule. La valeur par défaut est false.

```csharp
[Obsolete("This property is not used, please remove this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsCellAutoFit { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. Au lieu de cela, cette propriété n'est pas utilisée, veuillez supprimer cette propriété.. Cette propriété sera supprimée 12 mois plus tard depuis août 2022. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyIsCellAutoFitDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir un texte d'exemple qui dépasse la largeur de colonne par défaut
            worksheet.Cells["B4"].Value = "This is a long text that demonstrates cell autofit behavior when converting to image.";
            
            // Créer des options de rendu d'image
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Démontrer IsCellAutoFit false (par défaut)
            Console.WriteLine("Default IsCellAutoFit value: " + options.IsCellAutoFit);
            SaveAsImage(worksheet, options, "WithoutAutoFit.png");

            // Modifier IsCellAutoFit en true
            options.IsCellAutoFit = true;
            Console.WriteLine("Modified IsCellAutoFit value: " + options.IsCellAutoFit);
            SaveAsImage(worksheet, options, "WithAutoFit.png");

            Console.WriteLine("Images created successfully. Compare column widths in output files.");
        }

        private static void SaveAsImage(Worksheet worksheet, ImageOrPrintOptions options, string fileName)
        {
            // Configurer le format d'image
            options.ImageType = ImageType.Png;

            // Rendre la feuille de calcul en image avec les options spécifiées
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, fileName);
        }
    }
}
```

### Voir aussi

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


