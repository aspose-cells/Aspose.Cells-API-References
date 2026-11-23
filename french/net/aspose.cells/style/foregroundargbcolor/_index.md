---
title: "Style.ForegroundArgbColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Obtient et définit la couleur de premier plan avec une valeur ARGB 32 bits"
type: docs
url: /fr/net/aspose.cells/style/foregroundargbcolor/
---
## Style.ForegroundArgbColor property

Obtient et définit la couleur de premier plan avec une valeur ARGB 32 bits.

```csharp
public int ForegroundArgbColor { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyForegroundArgbColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer un style avec une couleur de premier plan spécifique
            Style style = workbook.CreateStyle();
            style.ForegroundColor = System.Drawing.Color.FromArgb(255, 0, 255, 0); // Green color
            style.Pattern = BackgroundType.Solid;
            
            // Appliquer le style à une cellule
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // Obtenir et afficher la valeur ARGB de la couleur de premier plan
            int foregroundArgb = cell.GetStyle().ForegroundArgbColor;
            Console.WriteLine("Foreground ARGB Color: " + foregroundArgb);
            
            // Enregistrez le classeur
            workbook.Save("ForegroundColorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


