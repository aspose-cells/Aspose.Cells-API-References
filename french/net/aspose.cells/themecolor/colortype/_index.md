---
title: "ThemeColor.ColorType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThemeColor. Obtient et définit le type de thème"
type: docs
url: /fr/net/aspose.cells/themecolor/colortype/
---
## ThemeColor.ColorType property

Obtient et définit le type de thème.

```csharp
public ThemeColorType ColorType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThemeColorPropertyColorTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créez deux couleurs de thème avec des types différents
            ThemeColor color1 = new ThemeColor(ThemeColorType.Accent1, 0.5);
            ThemeColor color2 = new ThemeColor(ThemeColorType.Accent2, 0.3);
            
            // Démontrez la propriété ColorType
            Console.WriteLine("Color1 Type: " + color1.ColorType);
            Console.WriteLine("Color2 Type: " + color2.ColorType);
            
            // Appliquez les couleurs de thème aux cellules
            Style style1 = workbook.CreateStyle();
            style1.ForegroundThemeColor = color1;
            worksheet.Cells["A1"].SetStyle(style1);
            
            Style style2 = workbook.CreateStyle();
            style2.ForegroundThemeColor = color2;
            worksheet.Cells["A2"].SetStyle(style2);
            
            // Enregistrez le classeur
            workbook.Save("ThemeColorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ThemeColorType](../../themecolortype/)
* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


