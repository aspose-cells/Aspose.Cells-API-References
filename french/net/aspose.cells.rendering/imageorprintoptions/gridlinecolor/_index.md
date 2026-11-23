---
title: "ImageOrPrintOptions.GridlineColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageOrPrintOptions. Obtient ou définit la couleur de la ligne de grille"
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/gridlinecolor/
---
## ImageOrPrintOptions.GridlineColor property

Obtient ou définit la couleur de la ligne de grille.

```csharp
public Color GridlineColor { get; set; }
```

### Remarques

Il ignorera les paramètres de couleur des lignes de grille dans le fichier source.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing;

    public class ImageOrPrintOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple afin que la feuille de calcul contienne du contenu
            worksheet.Cells["A1"].PutValue("Demo for GridlineColor property");

            try
            {
                // Créer une instance de ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Affichez la valeur actuelle de GridlineColor (lecture‑seule ou lecture/écriture)
                // Le type de la propriété est supposé être System.Drawing.Color
                Console.WriteLine("Current GridlineColor: " + options.GridlineColor);

                // Rendez éventuellement la feuille en image pour voir l'effet de la couleur de ligne de grille par défaut
                // (Pas besoin de changer la valeur ; nous montrons simplement l'utilisation.)
                SheetRender renderer = new SheetRender(worksheet, options);
                renderer.ToImage(0, "GridlineColorDemo.png");

                // Enregistrer le classeur (facultatif)
                workbook.Save("GridlineColorDemo.xlsx");

                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during demo: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


