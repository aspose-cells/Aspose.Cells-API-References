---
title: "Cells.StandardWidthPixels"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul en unité de pixels"
type: docs
url: /fr/net/aspose.cells/cells/standardwidthpixels/
---
## Cells.StandardWidthPixels property

Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul, en pixels.

```csharp
public int StandardWidthPixels { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthPixelsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir et obtenir la largeur standard en pixels
            cells.StandardWidthPixels = 104;
            Console.WriteLine("Standard Width in Pixels: " + cells.StandardWidthPixels);

            // Définir et obtenir la largeur standard en caractères
            cells.StandardWidth = 12.375;
            Console.WriteLine("Standard Width in Characters: " + cells.StandardWidth);

            // Définir et obtenir la hauteur standard en points
            cells.StandardHeight = 14.25;
            Console.WriteLine("Standard Height in Points: " + cells.StandardHeight);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


