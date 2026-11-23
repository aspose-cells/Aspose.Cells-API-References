---
title: "Style.ForegroundThemeColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Obtient et définit la couleur de thème d'avant-plan"
type: docs
url: /fr/net/aspose.cells/style/foregroundthemecolor/
---
## Style.ForegroundThemeColor property

Obtient et définit la couleur du thème de premier plan.

```csharp
public ThemeColor ForegroundThemeColor { get; set; }
```

### Remarques

Si la couleur d'avant-plan n'est pas une couleur de thème, NULL sera retourné.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyForegroundThemeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            cells["A1"].PutValue("Foreground Theme Color Demo");
            Style style = cells["A1"].GetStyle();

            style.ForegroundThemeColor = new ThemeColor(ThemeColorType.Accent1, -0.25);
            style.Pattern = BackgroundType.Solid;

            cells["A1"].SetStyle(style);
            workbook.Save("ForegroundThemeColorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ThemeColor](../../themecolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


