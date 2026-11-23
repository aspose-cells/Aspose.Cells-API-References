---
title: "Cells.StandardHeightPixels"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul en unités de pixels"
type: docs
url: /fr/net/aspose.cells/cells/standardheightpixels/
---
## Cells.StandardHeightPixels property

Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en pixels.

```csharp
public int StandardHeightPixels { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightPixelsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir certaines données dans les cellules
            cells["A1"].PutValue("Sample Data");
            cells["B2"].PutValue(123);
            cells["C3"].PutValue(DateTime.Now);

            // Obtenir la hauteur standard en pixels
            int standardHeight = cells.StandardHeightPixels;
            Console.WriteLine("Standard row height in pixels: " + standardHeight);

            // Afficher les hauteurs des lignes (doit correspondre à la hauteur standard)
            for (int i = 0; i < 5; i++)
            {
                int rowHeight = cells.GetRowHeightPixel(i);
                Console.WriteLine($"Row {i} height: {rowHeight}px");
                Console.WriteLine($"Matches standard: {rowHeight == standardHeight}");
            }

            // Modifier la hauteur standard et vérifier
            cells.StandardHeight = 20; // Set in points
            int newStandardHeight = cells.StandardHeightPixels;
            Console.WriteLine("\nNew standard height in pixels: " + newStandardHeight);

            // Vérifier que toutes les lignes ont maintenant la nouvelle hauteur
            for (int i = 0; i < 5; i++)
            {
                int rowHeight = cells.GetRowHeightPixel(i);
                Console.WriteLine($"Row {i} height: {rowHeight}px");
                Console.WriteLine($"Matches new standard: {rowHeight == newStandardHeight}");
            }
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


