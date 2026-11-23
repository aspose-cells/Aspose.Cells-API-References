---
title: "StyleFlag.Borders"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Tous les paramètres de bordures seront appliqués"
type: docs
url: /fr/net/aspose.cells/styleflag/borders/
---
## StyleFlag.Borders property

Tous les paramètres de bordure seront appliqués.

```csharp
public bool Borders { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyBordersDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créer un style avec des paramètres de bordure
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].Color = System.Drawing.Color.Blue;

            // Créer un style flag et activer les bordures
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;

            // Appliquer le style à la cellule A1 avec uniquement les bordures
            cells["A1"].PutValue("Borders Demo");
            cells["A1"].SetStyle(style, styleFlag);

            // Enregistrez le classeur
            workbook.Save("BordersDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


