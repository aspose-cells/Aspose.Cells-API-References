---
title: "Worksheet.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar eller anger namnet på kalkylbladet"
type: docs
url: /sv/net/aspose.cells/worksheet/name/
---
## Worksheet.Name property

Hämtar eller anger namnet på arbetsbladet.

```csharp
public string Name { get; set; }
```

### Anmärkningar

Den maximala längden för bladnamn är 31. Och du kan inte tilldela samma namn (skiftlägesokänsligt) till två kalkylblad. Till exempel kan du inte sätta "SheetName1" på det första kalkylbladet och sätta "SHEETNAME1" på det andra kalkylbladet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Få åtkomst till det första kalkylbladet och ange dess namn
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // Lägg till ett nytt kalkylblad med ett specifikt namn
            Worksheet newSheet = workbook.Worksheets.Add("ReportSheet");
            
            // Skriv ut namnen på alla kalkylblad
            Console.WriteLine("Worksheet Names:");
            foreach (Worksheet ws in workbook.Worksheets)
            {
                Console.WriteLine(ws.Name);
            }
            
            // Spara arbetsboken
            workbook.Save("WorksheetNamesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


