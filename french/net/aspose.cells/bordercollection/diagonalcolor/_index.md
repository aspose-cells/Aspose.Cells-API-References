---
title: "BorderCollection.DiagonalColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BorderCollection. Obtient ou définit la couleur des lignes diagonales"
type: docs
url: /fr/net/aspose.cells/bordercollection/diagonalcolor/
---
## BorderCollection.DiagonalColor property

Obtient ou définit la Couleur des lignes Diagonales.

```csharp
public Color DiagonalColor { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BorderCollectionPropertyDiagonalColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Diagonal Border Demo");

            Style style = cell.GetStyle();
            
            // Définition des propriétés de bordure diagonale
            style.Borders.DiagonalColor = Color.Red;
            style.Borders.DiagonalStyle = CellBorderType.Thick;

            cell.SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("DiagonalBorderDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


