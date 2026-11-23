---
title: "PdfSaveOptions.ImageType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PdfSaveOptions. Représente le type d’image lors de la conversion du graphique et de la forme"
type: docs
url: /fr/net/aspose.cells/pdfsaveoptions/imagetype/
---
## PdfSaveOptions.ImageType property

Représente le type d’image lors de la conversion du graphique et de la forme.

```csharp
[Obsolete("Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ImageFormat ImageType { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, Chart et Shape sont toujours rendus comme des éléments vectoriels (par ex. point, ligne) pour la qualité du rendu. Cette propriété sera supprimée 12 mois plus tard, depuis juin 2022. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing.Imaging;

    public class PdfSaveOptionsPropertyImageTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Créer une feuille de calcul d’exemple avec quelques données
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data for PDF Export";
            worksheet.Cells["A2"].Value = "Demonstrating ImageType Property";

            try
            {
                // Créez les options d'enregistrement PDF
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // Afficher la valeur par défaut de ImageType
                Console.WriteLine("Default ImageType: " + saveOptions.ImageType);

                // Définir une valeur différente pour ImageType
                saveOptions.ImageType = ImageFormat.Png;
                Console.WriteLine("Updated ImageType: " + saveOptions.ImageType);

                // Enregistrer le classeur au format PDF avec le ImageType spécifié
                workbook.Save("ImageTypeDemo.pdf", saveOptions);

                Console.WriteLine("PDF saved with ImageType setting applied.");
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

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


