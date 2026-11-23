---
title: "ThemeColor.Tint"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThemeColor. Obtient et définit la valeur de teinte"
type: docs
url: /fr/net/aspose.cells/themecolor/tint/
---
## ThemeColor.Tint property

Obtient et définit la valeur de teinte.

```csharp
public double Tint { get; set; }
```

### Remarques

La valeur de teinte est stockée sous forme de double de -1.0 à 1.0, où -1.0 signifie 100 % assombrissement et 1.0 signifie 100 % éclaircissement. De plus, 0.0 signifie aucun changement.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThemeColorPropertyTintDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez un style avec la couleur du thème et la teinte
            Style style = workbook.CreateStyle();
            style.BackgroundThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5); // 0.5 tint
            
            // Appliquer le style à une cellule
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);

            // Obtenez la valeur de teinte à partir du style de la cellule
            double tintValue = cell.GetStyle().BackgroundThemeColor.Tint;
            Console.WriteLine("Tint value: " + tintValue);

            // Modifiez la valeur de teinte
            ThemeColor themeColor = cell.GetStyle().BackgroundThemeColor;
            themeColor.Tint = 0.8; // Change tint to 0.8
            cell.SetStyle(style);

            // Vérifiez la nouvelle valeur de teinte
            Console.WriteLine("Modified tint value: " + cell.GetStyle().BackgroundThemeColor.Tint);
        }
    }
}
```

### Voir aussi

* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


