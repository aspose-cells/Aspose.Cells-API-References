---
title: "Border.ThemeColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Border. Obtient et définit la couleur du thème de la bordure"
type: docs
url: /fr/net/aspose.cells/border/themecolor/
---
## Border.ThemeColor property

Obtient et définit la couleur de thème de la bordure.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyThemeColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à une cellule et obtenir son style
            Style style = worksheet.Cells["A1"].GetStyle();

            // Définir la couleur du thème de la bordure
            style.Borders[BorderType.BottomBorder].ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            // Appliquez le style à la cellule
            worksheet.Cells["A1"].SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("BorderThemeColorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ThemeColor](../../themecolor/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


