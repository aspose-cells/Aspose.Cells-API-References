---
title: "BorderCollection.DiagonalStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BorderCollection. Obtient ou définit le style des lignes diagonales"
type: docs
url: /fr/net/aspose.cells/bordercollection/diagonalstyle/
---
## BorderCollection.DiagonalStyle property

Obtient ou définit le style des lignes Diagonales.

```csharp
public CellBorderType DiagonalStyle { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BorderCollectionPropertyDiagonalStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenir une cellule et son style
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            
            // Définir les propriétés de la bordure diagonale
            style.Borders.DiagonalStyle = CellBorderType.Thin;
            style.Borders.DiagonalColor = Color.Red;
            
            // Appliquez le style à la cellule
            cell.SetStyle(style);
            
            // Enregistrez le classeur
            workbook.Save("DiagonalBorderDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


