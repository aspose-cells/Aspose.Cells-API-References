---
title: "UnionRange.Value"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété UnionRange. Obtient et définit les valeurs de la plage"
type: docs
url: /fr/net/aspose.cells/unionrange/value/
---
## UnionRange.Value property

Obtient et définit les valeurs de la plage.

```csharp
public object Value { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class UnionRangePropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crée une plage d'union en utilisant l'API correcte
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:B2,D1:E2", 0);
            
            // Définit la valeur pour l'ensemble de la plage d'union
            unionRange.Value = "Test Value";
            
            // Créez et appliquez le style
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            unionRange.ApplyStyle(style, new StyleFlag { All = true });
            
            // Enregistrez le classeur
            workbook.Save("UnionRangeValueDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


