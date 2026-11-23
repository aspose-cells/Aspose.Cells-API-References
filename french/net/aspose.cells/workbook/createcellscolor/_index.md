---
title: "Workbook.CreateCellsColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Crée un objet CellsColor"
type: docs
url: /fr/net/aspose.cells/workbook/createcellscolor/
---
## Workbook.CreateCellsColor method

Crée un objet [`CellsColor`](../../cellscolor/).

```csharp
public CellsColor CreateCellsColor()
```

### Valeur de retour

Renvoie un objet [`CellsColor`](../../cellscolor/).

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateCellsColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Créer une plage et définir les bordures avec une couleur personnalisée
            Aspose.Cells.Range range = workbook.Worksheets[0].Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Horizontal, CellBorderType.Thin, color);

            // Vérifier le style de bordure dans une cellule spécifique
            Cell cell = workbook.Worksheets[0].Cells["F5"];
            Style style = cell.GetStyle();
            Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
            Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);
            Console.WriteLine("Top Border: " + style.Borders[BorderType.TopBorder].LineStyle);
            Console.WriteLine("Right Border: " + style.Borders[BorderType.RightBorder].LineStyle);

            workbook.Save("CreateCellsColorExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [CellsColor](../../cellscolor/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


