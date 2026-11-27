---
title: "Worksheet.Workbook"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar arbetsboksobjektet som innehåller detta blad"
type: docs
url: /sv/net/aspose.cells/worksheet/workbook/
---
## Worksheet.Workbook property

Hämtar arbetsboksobjektet som innehåller detta blad.

```csharp
public Workbook Workbook { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyWorkbookDemo
    {
        public static void Run()
        {
            // Skapa en källarbetsbok och hämta ett arbetsblad
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Lägg till exempeldata i källarbetsbladet
            sourceSheet.Cells["A1"].PutValue("Sample Data");
            sourceSheet.Cells["A2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue(200);
            
            // Skapa en målarbetsbok
            Workbook destWorkbook = new Workbook();
            
            // Kopiera tema från källarbetsboken med hjälp av Worksheet.Workbook-egenskapen
            destWorkbook.CopyTheme(sourceSheet.Workbook);
            
            // Kom åt destinationsarbetsbladet och kopiera data
            Worksheet destSheet = destWorkbook.Worksheets[0];
            Aspose.Cells.Range sourceRange = sourceSheet.Cells.CreateRange("A1:A3");
            Aspose.Cells.Range destRange = destSheet.Cells.CreateRange("A1:A3");
            
            // Kopiera data med formatering
            destRange.Copy(sourceRange);
            
            // Spara målarbetsboken
            destWorkbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Workbook](../../workbook/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


