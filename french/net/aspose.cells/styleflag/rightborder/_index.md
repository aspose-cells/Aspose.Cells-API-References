---
title: "StyleFlag.RightBorder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Les paramètres de bordure droite seront appliqués"
type: docs
url: /fr/net/aspose.cells/styleflag/rightborder/
---
## StyleFlag.RightBorder property

Les paramètres de bordure droite seront appliqués.

```csharp
public bool RightBorder { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyRightBorderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un style avec des bordures
            Style borderStyle = workbook.CreateStyle();
            borderStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            borderStyle.Borders[BorderType.RightBorder].Color = System.Drawing.Color.Red;

            // Créer un indicateur de style et activer la bordure droite
            StyleFlag borderFlag = new StyleFlag();
            borderFlag.RightBorder = true;

            // Appliquer le style à une cellule
            Cell cell = worksheet.Cells["B2"];
            cell.SetStyle(borderStyle, borderFlag);

            // Enregistrez le classeur
            workbook.Save("RightBorderDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


