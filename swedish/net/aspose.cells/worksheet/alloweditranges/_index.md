---
title: "Worksheet.AllowEditRanges"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar samlingen av tillåtna redigeringsområden i kalkylbladet"
type: docs
url: /sv/net/aspose.cells/worksheet/alloweditranges/
---
## Worksheet.AllowEditRanges property

Hämtar samlingen för tillåtna redigeringsområden i kalkylbladet.

```csharp
public ProtectedRangeCollection AllowEditRanges { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyAllowEditRangesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett tillåtet redigeringsområde
            int index = worksheet.AllowEditRanges.Add("r1", 0, 0, 1, 1);
            ProtectedRange range = worksheet.AllowEditRanges[index];
            range.Password = "password123";

            // Skydda kalkylbladet
            worksheet.Protect(ProtectionType.All);

            // Spara arbetsboken
            workbook.Save("output.xlsx");

            // Läs in den sparade arbetsboken för att verifiera
            Workbook verifyWorkbook = new Workbook("output.xlsx");
            ProtectedRange verifyRange = verifyWorkbook.Worksheets[0].AllowEditRanges[0];
            Console.WriteLine("Is protected with password: " + verifyRange.IsProtectedWithPassword);
        }
    }
}
```

### Se även

* class [ProtectedRangeCollection](../../protectedrangecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


