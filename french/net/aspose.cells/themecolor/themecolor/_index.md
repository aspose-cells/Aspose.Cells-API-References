---
title: "ThemeColor.ThemeColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur ThemeColor."
type: docs
url: /fr/net/aspose.cells/themecolor/themecolor/
---
## ThemeColor constructor

```csharp
public ThemeColor(ThemeColorType type, double tint)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | ThemeColorType | Le type de thème. |
| teinte | Double | La valeur de teinte. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThemeColorMethodCtorWithThemeColorTypeDoubleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Appelez la méthode #ctor avec les paramètres ThemeColorType et Double
                ThemeColor themeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

                // Appliquez la couleur du thème au style d'une cellule
                Style style = workbook.CreateStyle();
                style.ForegroundThemeColor = themeColor;
                style.Pattern = BackgroundType.Solid;
                
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("ThemeColor with Accent1 and 0.5 tint");
                cell.SetStyle(style);

                Console.WriteLine("ThemeColor constructor executed successfully with parameters (ThemeColorType.Accent1, 0.5)");
                Console.WriteLine($"ColorType: {themeColor.ColorType}, Tint: {themeColor.Tint}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ThemeColor constructor: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("ThemeColorCtorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ThemeColorType](../../themecolortype/)
* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


