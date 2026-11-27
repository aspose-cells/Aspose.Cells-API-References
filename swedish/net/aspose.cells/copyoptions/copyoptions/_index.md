---
title: "CopyOptions.CopyOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CopyOptions‑konstruktor. CopyOptions‑konstruktor"
type: docs
url: /sv/net/aspose.cells/copyoptions/copyoptions/
---
## CopyOptions constructor

CopyOptions-konstruktor.

```csharp
public CopyOptions()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad och hämta det första kalkylbladet
            Worksheet sourceSheet = workbook.Worksheets[0];
            Worksheet destSheet = workbook.Worksheets[workbook.Worksheets.Add()];
            
            // Lägg till exempeldata i källbladet
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["A2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue(200);
            sourceSheet.Cells["A4"].PutValue(300);
            
            // Skapa CopyOptions med konstruktorn
            CopyOptions options = new CopyOptions();
            options.ReferToDestinationSheet = true;
            
            // Kopiera rader med alternativen
            destSheet.Cells.CopyRows(sourceSheet.Cells, 0, 0, sourceSheet.Cells.MaxDisplayRange.RowCount, options);
            
            // Spara arbetsboken
            workbook.Save("CopyOptionsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


