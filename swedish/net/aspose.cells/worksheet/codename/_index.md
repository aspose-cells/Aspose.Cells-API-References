---
title: "Worksheet.CodeName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet‑egenskap. Hämtar kalkylbladets kodnamn"
type: docs
url: /sv/net/aspose.cells/worksheet/codename/
---
## Worksheet.CodeName property

Hämtar kalkylbladets kodnamn.

```csharp
public string CodeName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCodeNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Visa standard‑CodeName
            Console.WriteLine("Default CodeName: " + worksheet.CodeName);
            
            // Ändra CodeName
            worksheet.CodeName = "MySheet";
            Console.WriteLine("Modified CodeName: " + worksheet.CodeName);
            
            // Lägg till ett nytt kalkylblad och visa dess CodeName
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            Console.WriteLine("New Sheet CodeName: " + newSheet.CodeName);
            
            // Spara arbetsboken
            workbook.Save("WorksheetCodeNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


