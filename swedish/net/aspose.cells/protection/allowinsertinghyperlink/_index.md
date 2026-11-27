---
title: "Protection.AllowInsertingHyperlink"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Protection-egenskap. Representerar om infogning av hyperlänkar är tillåten i ett skyddat kalkylblad"
type: docs
url: /sv/net/aspose.cells/protection/allowinsertinghyperlink/
---
## Protection.AllowInsertingHyperlink property

Representerar om infogning av hyperlänkar är tillåten på ett skyddat kalkylblad

```csharp
public bool AllowInsertingHyperlink { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingHyperlinkDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Protection protection = worksheet.Protection;
            protection.AllowInsertingHyperlink = true;
            protection.Password = "password123";

            // Lägg till en hyperlänk för att demonstrera funktionen
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            workbook.Save("AllowInsertingHyperlinkDemo.xlsx");
        }
    }
}
```

### Se även

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


