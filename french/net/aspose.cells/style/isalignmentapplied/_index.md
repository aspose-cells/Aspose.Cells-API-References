---
title: "Style.IsAlignmentApplied"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Indique si le formatage d'alignement doit être appliqué"
type: docs
url: /fr/net/aspose.cells/style/isalignmentapplied/
---
## Style.IsAlignmentApplied property

Indique si le formatage d'alignement doit être appliqué.

```csharp
public bool IsAlignmentApplied { get; set; }
```

### Remarques

Uniquement pour le style nommé.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsAlignmentAppliedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            
            // Définissez les propriétés d'alignement
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            
            // Activez l'application de l'alignement
            style.IsAlignmentApplied = true;
            
            cell.SetStyle(style);
            
            // Vérifiez que l'alignement est appliqué
            Console.WriteLine("Alignment applied: " + style.IsAlignmentApplied);
            Console.WriteLine("Horizontal Alignment: " + style.HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + style.VerticalAlignment);
            
            workbook.Save("AlignmentExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


