---
title: "Enum TargetModeType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.TargetModeType enum. Representerar typen av mål-läge"
type: docs
url: /sv/net/aspose.cells/targetmodetype/
---
## TargetModeType enumeration

Representerar typen av målläge.

```csharp
public enum TargetModeType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| External | `0` | Extern länk |
| FilePath | `1` | Lokala och fullständiga sökvägar till filer eller mappar. |
| Email | `2` | E‑post. |
| CellReference | `3` | Länk på cell eller namngivet område. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTargetModeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en extern hyperlänk
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Hämta hyperlänken och kontrollera dess TargetModeType
            Hyperlink link = worksheet.Hyperlinks[0];
            Console.WriteLine("Hyperlink TargetModeType: " + link.LinkType);
            
            // Ta bort hyperlänken
            link.Delete();
            Console.WriteLine("Hyperlinks count after deletion: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


