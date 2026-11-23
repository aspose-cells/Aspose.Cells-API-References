---
title: "ImageOrPrintOptions.AllColumnsInOnePagePerSheet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageOrPrintOptions. Si AllColumnsInOnePagePerSheet est vrai, tout le contenu des colonnes d’une feuille sera généré sur une seule page dans le résultat. La largeur du format de papier du paramètre pagesetup sera invalide et les autres paramètres du pagesetup resteront appliqués."
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/
---
## ImageOrPrintOptions.AllColumnsInOnePagePerSheet property

Si AllColumnsInOnePagePerSheet est vrai, tout le contenu des colonnes d'une feuille sera exporté sur une seule page dans le résultat. La largeur du format de papier du paramètre pagesetup sera invalide, et les autres paramètres de pagesetup resteront effectifs.

```csharp
public bool AllColumnsInOnePagePerSheet { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyAllColumnsInOnePagePerSheetDemo
    {
        public static void Run()
        {
            // Créez un classeur et ajoutez des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplissez quelques données dans la feuille de calcul
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Créer des options d’enregistrement d’image
            ImageSaveOptions pngOptions = new ImageSaveOptions(SaveFormat.Png);
            pngOptions.ImageOrPrintOptions.AllColumnsInOnePagePerSheet = true;
            pngOptions.ImageOrPrintOptions.OnePagePerSheet = true;

            // Enregistrer le classeur dans un flux mémoire au format PNG
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, pngOptions);
                Console.WriteLine("Workbook saved as PNG with all columns in one page per sheet.");
            }
        }
    }
}
```

### Voir aussi

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


