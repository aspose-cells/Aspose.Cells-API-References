---
title: "Cells.SetViewColumnWidthPixel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Définit la largeur de la colonne dans différentes vues"
type: docs
url: /fr/net/aspose.cells/cells/setviewcolumnwidthpixel/
---
## Cells.SetViewColumnWidthPixel method

Définit la largeur de la colonne dans différentes vues.

```csharp
public void SetViewColumnWidthPixel(int column, int pixels)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| column | Int32 | L'index de colonne. |
| pixels | Int32 | La largeur en unité de pixels. |

### Remarques

Si le type de vue actuel est PageLayoutView, la largeur de la colonne est identique à la largeur imprimée.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetViewColumnWidthPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Définir des données d'exemple
            sheet.Cells[0, 0].Value = "Sample Text";

            // Calculez la largeur en pixels (100 pixels dans cet exemple)
            int pixelWidth = 100;

            // Définissez la largeur de la colonne en pixels
            sheet.Cells.SetViewColumnWidthPixel(0, pixelWidth);

            // Enregistrez le classeur
            wb.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


