---
title: "Style.SetPatternColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Style. Définit la couleur d'arrière-plan"
type: docs
url: /fr/net/aspose.cells/style/setpatterncolor/
---
## Style.SetPatternColor method

Définit la couleur d'arrière-plan.

```csharp
public void SetPatternColor(BackgroundType pattern, Color color1, Color color2)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| motif | BackgroundType | Le motif. |
| color1 | Color | La couleur de premier plan. |
| color2 | Color | La couleur d'arrière-plan. Fonctionne uniquement lorsque le motif n'est pas BackgroundType.None et BackgroundType.Solid. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleMethodSetPatternColorWithBackgroundTypeColorColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            style.SetPatternColor(BackgroundType.Solid, Color.Red, Color.Blue);
            cell.SetStyle(style);
            
            workbook.Save("SetPatternColorDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


