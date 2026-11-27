---
title: "Enum GridlineType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridlineType enum. Enumererar rutnätslinjetyp"
type: docs
url: /sv/net/aspose.cells/gridlinetype/
---
## GridlineType enumeration

Enumererar rutnätslinjetyp.

```csharp
public enum GridlineType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Dotted | `0` | Representerar streckad linje. |
| Hair | `1` | Representerar hårlinje. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassGridlineTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa sparalternativ och ange rutnätslinjetyp
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.GridlineType = GridlineType.Dotted;
            
            // Lägg till exempeldata för att se rutnätslinjer
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B2"].PutValue(123);
            worksheet.Cells["C3"].PutValue(DateTime.Now);
            
            // Spara arbetsboken med sparalternativen
            workbook.Save("GridlineTypeDemo.docx", saveOptions);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


