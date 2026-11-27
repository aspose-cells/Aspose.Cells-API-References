---
title: "ExternalLink.AddExternalName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalLink-metod. Lägger till ett externt namn"
type: docs
url: /sv/net/aspose.cells/externallink/addexternalname/
---
## ExternalLink.AddExternalName method

Lägger till ett externt namn.

```csharp
public void AddExternalName(string text, string referTo)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | String | Texten för det externa namnet. Om det externa namnet tillhör ett kalkylblad ska texten vara som Sheet1!Text. |
| referTo | String | ReferTo för det externa namnet. Det måste vara en cell eller ett område. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkMethodAddExternalNameWithStringStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Skapa en exempelarbetsbok externt
            Workbook externalWorkbook = new Workbook();
            Worksheet externalSheet = externalWorkbook.Worksheets[0];
            externalSheet.Cells["B2"].PutValue(67);
            
            // Lägg till extern länk till huvudarbetsboken
            string[] sheetNames = new string[] { externalSheet.Name };
            int index = workbook.Worksheets.ExternalLinks.Add("ExternalWorkbook.xlsx", sheetNames);
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[index];
            
            // Lägg till externt namn
            externalLink.AddExternalName("Test", "=Sheet1!$B$2");
            
            // Använd det externa namnet i en formel
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].Formula = "=[ExternalWorkbook.xlsx]!Test";
            
            // Beräkna formeln
            workbook.CalculateFormula();
            
            // Skriv ut resultatet
            Console.WriteLine("Value from external reference: " + sheet.Cells["A1"].DoubleValue);
        }
    }
}
```

### Se även

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


