---
title: "UnionRange.HasRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété UnionRange. Indique si cela possède une plage"
type: docs
url: /fr/net/aspose.cells/unionrange/hasrange/
---
## UnionRange.HasRange property

Indique si cela possède une plage.

```csharp
public bool HasRange { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class UnionRangePropertyHasRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crée une plage d'union en utilisant l'API correcte
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A5,B1:B5", 0);
            
            // Vérifier si la plage d'union possède des plages valides
            Console.WriteLine("UnionRange has ranges: " + unionRange.HasRange);
            
            // Définir la valeur et le style uniquement si la plage est valide
            if (unionRange.HasRange)
            {
                unionRange.Value = "Test Value";
                
                Style style = workbook.CreateStyle();
                style.Pattern = BackgroundType.Solid;
                style.ForegroundColor = System.Drawing.Color.LightBlue;
                unionRange.ApplyStyle(style, new StyleFlag { All = true });
            }
            
            workbook.Save("UnionRangeHasRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


