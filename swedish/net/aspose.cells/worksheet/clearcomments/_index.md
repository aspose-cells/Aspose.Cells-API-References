---
title: "Worksheet.ClearComments"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Rensar alla kommentarer i designerns kalkylblad"
type: docs
url: /sv/net/aspose.cells/worksheet/clearcomments/
---
## Worksheet.ClearComments method

Rensar alla kommentarer i designerns kalkylblad.

```csharp
public void ClearComments()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodClearCommentsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempelkommentarer i celler med hjälp av cellreferenser
            int comment1 = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1].Note = "This is comment 1";
            
            int comment2 = worksheet.Comments.Add("B3");
            worksheet.Comments[comment2].Note = "This is comment 2";
            
            int comment3 = worksheet.Comments.Add("C5");
            worksheet.Comments[comment3].Note = "This is comment 3";

            // Visa antalet kommentarer innan rensning
            Console.WriteLine($"Comments count before ClearComments(): {worksheet.Comments.Count}");

            // Rensa alla kommentarer från kalkylbladet
            worksheet.ClearComments();

            // Visa antalet kommentarer efter rensning
            Console.WriteLine($"Comments count after ClearComments(): {worksheet.Comments.Count}");

            // Spara arbetsboken
            workbook.Save("ClearCommentsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


