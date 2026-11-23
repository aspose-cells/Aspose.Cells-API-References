---
title: "Style.Pattern"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Obtient ou définit le type de motif d'arrière-plan de la cellule"
type: docs
url: /fr/net/aspose.cells/style/pattern/
---
## Style.Pattern property

Obtient ou définit le type de motif d'arrière-plan de la cellule.

```csharp
public BackgroundType Pattern { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyPatternDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Accéder à la cellule et obtenir son style
            Cell cell = cells[0, 0];
            Style style = cell.GetStyle();
            
            // Définir le motif et la couleur de premier plan
            style.Pattern = BackgroundType.Gray50;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            
            // Appliquez le style à la cellule
            cell.SetStyle(style);
            
            // Enregistrez le classeur
            workbook.Save("PatternPropertyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


