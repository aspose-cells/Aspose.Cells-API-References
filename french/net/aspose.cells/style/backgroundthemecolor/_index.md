---
title: "Style.BackgroundThemeColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Obtient et définit la couleur de thème d'arrière-plan"
type: docs
url: /fr/net/aspose.cells/style/backgroundthemecolor/
---
## Style.BackgroundThemeColor property

Obtient et définit la couleur du thème d'arrière-plan.

```csharp
public ThemeColor BackgroundThemeColor { get; set; }
```

### Remarques

Si la couleur d'arrière-plan n'est pas une couleur de thème, NULL sera retourné.

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyBackgroundThemeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créer un style et définir la couleur de thème d'arrière-plan
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            
            ThemeColor themeColor = new ThemeColor(ThemeColorType.Accent2, 0.5);
            style.BackgroundThemeColor = themeColor;

            // Appliquer le style à une cellule
            cells["A1"].SetStyle(style);

            // Vérifier la couleur de thème d'arrière-plan
            ThemeColor retrievedColor = cells["A1"].GetStyle().BackgroundThemeColor;
            Console.WriteLine("Background Theme Color Type: " + retrievedColor.ColorType);
            Console.WriteLine("Background Theme Color Tint: " + retrievedColor.Tint);
        }
    }
}
```

### Voir aussi

* class [ThemeColor](../../themecolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


