---
title: "BorderCollection.SetStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode BorderCollection. Définit le style de toutes les bordures de la collection"
type: docs
url: /fr/net/aspose.cells/bordercollection/setstyle/
---
## BorderCollection.SetStyle method

Définit le style de toutes les bordures de la collection.

```csharp
public void SetStyle(CellBorderType style)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| style | CellBorderType | Style des bordures |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderCollectionMethodSetStyleWithCellBorderTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenir la cellule C6 et son style
            Cell cell = worksheet.Cells["C6"];
            Style style = cell.GetStyle();

            // Définir la couleur et le style de la bordure
            style.Borders.SetColor(System.Drawing.Color.Red);
            style.Borders.SetStyle(CellBorderType.Thick);

            // Appliquez le style à la cellule
            cell.SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("BorderCollectionMethodSetStyleWithCellBorderTypeDemo_out.xlsx");

            Console.WriteLine("Border style set successfully.");
        }
    }
}
```

### Voir aussi

* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


