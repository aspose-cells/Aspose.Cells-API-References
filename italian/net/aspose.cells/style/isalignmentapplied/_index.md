---
title: "Style.IsAlignmentApplied"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Indica se la formattazione di allineamento deve essere applicata"
type: docs
url: /it/net/aspose.cells/style/isalignmentapplied/
---
## Style.IsAlignmentApplied property

Indica se la formattazione dell'allineamento deve essere applicata.

```csharp
public bool IsAlignmentApplied { get; set; }
```

### Osservazioni

Solo per stile con nome.

### Esempi

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
            
            // Imposta le proprietà di allineamento
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            
            // Abilita l'applicazione dell'allineamento
            style.IsAlignmentApplied = true;
            
            cell.SetStyle(style);
            
            // Verifica che l'allineamento sia applicato
            Console.WriteLine("Alignment applied: " + style.IsAlignmentApplied);
            Console.WriteLine("Horizontal Alignment: " + style.HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + style.VerticalAlignment);
            
            workbook.Save("AlignmentExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


