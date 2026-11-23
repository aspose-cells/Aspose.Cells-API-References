---
title: "Font.ThemeColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Font. Obtient et définit la couleur du thème"
type: docs
url: /fr/net/aspose.cells/font/themecolor/
---
## Font.ThemeColor property

Obtient et définit la couleur du thème.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Remarques

Si la couleur de la police n'est pas une couleur de thème, NULL sera renvoyé.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyThemeColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accédez à la cellule A1 et définissez le texte
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Theme Color Demo");

            // Obtenez le style et la police
            Style style = cell.GetStyle();
            Font font = style.Font;

            // Créez et définissez la couleur du thème
            font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

            // Appliquez le style à la cellule
            cell.SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("ThemeColorDemo.xlsx");

            // Vérifiez la couleur du thème
            Font savedFont = worksheet.Cells["A1"].GetStyle().Font;
            Console.WriteLine("ThemeColor Type: " + savedFont.ThemeColor.ColorType);
            Console.WriteLine("ThemeColor Tint: " + savedFont.ThemeColor.Tint);
        }
    }
}
```

### Voir aussi

* class [ThemeColor](../../themecolor/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


