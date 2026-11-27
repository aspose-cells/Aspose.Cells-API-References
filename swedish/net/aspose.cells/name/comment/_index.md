---
title: "Name.Comment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Name-egenskap. Hämtar och anger kommentaren för namnet. Gäller endast för Excel 2007 eller senare versioner"
type: docs
url: /sv/net/aspose.cells/name/comment/
---
## Name.Comment property

Hämtar och anger kommentaren för namnet. Gäller endast för Excel 2007 eller senare versioner.

```csharp
public string Comment { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyCommentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till ett namngivet område med kommentar
            int index = workbook.Worksheets.Names.Add("TestRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$B$2";
            namedRange.Comment = "This is a test named range";
            
            // Spara arbetsboken
            workbook.Save("NamedRangeWithComment.xlsx");
            
            // Läs in den sparade arbetsboken för att verifiera kommentaren
            Workbook loadedWorkbook = new Workbook("NamedRangeWithComment.xlsx");
            Name loadedNamedRange = loadedWorkbook.Worksheets.Names[0];
            
            // Skriv ut kommentaren för att demonstrera funktionaliteten
            Console.WriteLine("Named Range Comment: " + loadedNamedRange.Comment);
        }
    }
}
```

### Se även

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


