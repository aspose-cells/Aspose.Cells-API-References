---
title: "Cells.GetViewColumnWidthPixel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient la largeur dans différents types de vue"
type: docs
url: /fr/net/aspose.cells/cells/getviewcolumnwidthpixel/
---
## Cells.GetViewColumnWidthPixel method

Obtenez la largeur dans différents types de vue.

```csharp
public int GetViewColumnWidthPixel(int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| column | Int32 | L'index de colonne. |

### Valeur de retour

la largeur de la colonne en unités de pixels

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetViewColumnWidthPixelWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir le type de vue sur PageLayoutView
            worksheet.ViewType = ViewType.PageLayoutView;
            
            // Définir la largeur de la colonne en caractères (sera convertie en pixels)
            worksheet.Cells.SetColumnWidth(0, 10);
            
            // Obtenir la largeur de la colonne en pixels
            int columnWidthInPixels = worksheet.Cells.GetViewColumnWidthPixel(0);
            
            // Afficher le résultat
            Console.WriteLine("Column width in pixels: " + columnWidthInPixels);
            
            // Enregistrez le classeur
            workbook.Save("ColumnWidthTest.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


