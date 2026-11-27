---
title: "ProtectedRange.GetAreas"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ProtectedRange-metod. Hämtar alla refererade områden"
type: docs
url: /sv/net/aspose.cells/protectedrange/getareas/
---
## ProtectedRange.GetAreas method

Hämtar alla refererade områden.

```csharp
public CellArea[] GetAreas()
```

### Returvärde

Returnerar alla refererade områden.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangeMethodGetAreasDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta samlingen av skyddade områden
            ProtectedRangeCollection protectedRanges = worksheet.AllowEditRanges;
            
            // Lägg till ett skyddat område
            int index = protectedRanges.Add("TestRange", 0, 0, 10, 10);
            ProtectedRange protectedRange = protectedRanges[index];
            
            // Hämta områdena för det skyddade området
            CellArea[] areas = protectedRange.GetAreas();
            
            // Skriv ut antalet områden (bör vara 1 för detta enkla område)
            Console.WriteLine("Number of areas in protected range: " + areas.Length);
            
            // Spara arbetsboken
            workbook.Save("ProtectedRangeExample.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


