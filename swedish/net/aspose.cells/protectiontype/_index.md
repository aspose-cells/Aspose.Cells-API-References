---
title: "Enum ProtectionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ProtectionType enum. Representerar skyddstyp för arbetsbok/arbetsblad"
type: docs
url: /sv/net/aspose.cells/protectiontype/
---
## ProtectionType enumeration

Representerar skyddstyp för arbetsbok/arbetsblad.

```csharp
public enum ProtectionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| All | `0` | Representerar att skydda allt. |
| Contents | `1` | Representerar att skydda innehåll, används i arbetsblads-skydd. |
| Objects | `2` | Representerar att skydda objekt, används i arbetsblads-skydd. |
| Scenarios | `3` | Representerar att skydda scenarier, används i arbetsblads-skydd. |
| Structure | `4` | Representerar att skydda struktur, används i arbetsboks-skydd. |
| Windows | `5` | Representerar att skydda fönster, används i arbetsboks-skydd. |
| None | `6` | Representerar inget skydd. Endast för egenskapen Reading. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassProtectionTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skydda arbetsbladet med alla skyddstyper
            worksheet.Protect(ProtectionType.All);
            
            // Demonstrera åtkomst till skyddsegenskaper
            Console.WriteLine("Worksheet protection settings:");
            Console.WriteLine("AllowDeletingColumn: " + worksheet.Protection.AllowDeletingColumn);
            Console.WriteLine("AllowDeletingRow: " + worksheet.Protection.AllowDeletingRow);
            Console.WriteLine("AllowFiltering: " + worksheet.Protection.AllowFiltering);
            Console.WriteLine("AllowFormattingCell: " + worksheet.Protection.AllowFormattingCell);
            Console.WriteLine("AllowFormattingColumn: " + worksheet.Protection.AllowFormattingColumn);
            Console.WriteLine("AllowFormattingRow: " + worksheet.Protection.AllowFormattingRow);
            Console.WriteLine("AllowInsertingColumn: " + worksheet.Protection.AllowInsertingColumn);
            Console.WriteLine("AllowInsertingHyperlink: " + worksheet.Protection.AllowInsertingHyperlink);
            Console.WriteLine("AllowInsertingRow: " + worksheet.Protection.AllowInsertingRow);
            Console.WriteLine("AllowSorting: " + worksheet.Protection.AllowSorting);
            Console.WriteLine("AllowUsingPivotTable: " + worksheet.Protection.AllowUsingPivotTable);
            
            // Ta bort skyddet från arbetsbladet
            worksheet.Unprotect();
            
            // Skydda med specifika skyddstyper
            worksheet.Protect(ProtectionType.Contents | ProtectionType.Objects);
            Console.WriteLine("\nWorksheet protected with Contents and Objects only");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


