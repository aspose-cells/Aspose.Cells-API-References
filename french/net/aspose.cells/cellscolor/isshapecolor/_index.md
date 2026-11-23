---
title: "CellsColor.IsShapeColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CellsColor. Obtient et définit la couleur qui doit s'appliquer à la cellule ou à la forme"
type: docs
url: /fr/net/aspose.cells/cellscolor/isshapecolor/
---
## CellsColor.IsShapeColor property

Obtient et définit la couleur qui doit être appliquée à la cellule ou à la forme.

```csharp
public bool IsShapeColor { get; set; }
```

### Remarques

L'expression de la couleur de la cellule et de la forme est différente. Par exemple : la couleur du thème avec la même valeur de teinte ne sera pas identique dans la cellule et la forme.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyIsShapeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une instance de CellsColor et définir IsShapeColor
            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.IsShapeColor = true;
            cellsColor.Color = Color.Green;

            // Appliquer la couleur à une forme
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = cellsColor.Color;  // Use the Color property instead of CellsColor directly

            // Enregistrez le classeur
            workbook.Save("CellsColorIsShapeColorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


