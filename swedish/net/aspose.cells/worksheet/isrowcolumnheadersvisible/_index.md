---
title: "Worksheet.IsRowColumnHeadersVisible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar eller anger ett värde som indikerar om kalkylbladet ska visa rad- och kolumnrubriker. Standard är true"
type: docs
url: /sv/net/aspose.cells/worksheet/isrowcolumnheadersvisible/
---
## Worksheet.IsRowColumnHeadersVisible property

Hämtar eller anger ett värde som indikerar om kalkylbladet ska visa rad- och kolumnrubriker. Standard är sant.

```csharp
public bool IsRowColumnHeadersVisible { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsRowColumnHeadersVisibleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in synligheten för rad- och kolumnrubriker till falskt
            worksheet.IsRowColumnHeadersVisible = false;
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Läs in den sparade arbetsboken för att verifiera egenskapen
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Skriv ut egenskapsvärdet
            Console.WriteLine("Row and Column Headers Visible: " + loadedWorksheet.IsRowColumnHeadersVisible);
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


