---
title: "Worksheet.VisibilityType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Anger det synliga tillståndet för detta blad"
type: docs
url: /sv/net/aspose.cells/worksheet/visibilitytype/
---
## Worksheet.VisibilityType property

Anger det synliga tillståndet för detta blad.

```csharp
public VisibilityType VisibilityType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyVisibilityTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till arbetsblad
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();

            // Ställ in olika synlighetstyper för varje arbetsblad
            workbook.Worksheets[0].VisibilityType = VisibilityType.Hidden;
            workbook.Worksheets[1].VisibilityType = VisibilityType.VeryHidden;
            workbook.Worksheets[2].VisibilityType = VisibilityType.Visible;

            // Spara arbetsboken
            string outputPath = "output_visibility.xlsx";
            workbook.Save(outputPath);

            // Läs in arbetsboken igen för att verifiera synlighetsinställningarna
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Skriv ut synlighetstyper
            Console.WriteLine("Worksheet 0 Visibility: " + loadedWorkbook.Worksheets[0].VisibilityType);
            Console.WriteLine("Worksheet 1 Visibility: " + loadedWorkbook.Worksheets[1].VisibilityType);
            Console.WriteLine("Worksheet 2 Visibility: " + loadedWorkbook.Worksheets[2].VisibilityType);
        }
    }
}
```

### Se även

* enum [VisibilityType](../../visibilitytype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


