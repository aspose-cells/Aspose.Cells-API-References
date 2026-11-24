---
title: "PageSetup.CenterHorizontally"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt an, ob das Blatt horizontal zentriert gedruckt wird"
type: docs
url: /de/net/aspose.cells/pagesetup/centerhorizontally/
---
## PageSetup.CenterHorizontally property

Gibt an, ob das Blatt horizontal zentriert gedruckt wird.

```csharp
public bool CenterHorizontally { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyCenterHorizontallyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Beispieldaten einfügen
            worksheet.Cells["A1"].PutValue("Sample Data");
            for (int i = 1; i <= 5; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + i);
                worksheet.Cells["B" + (i + 1)].PutValue(i * 100);
            }

            PageSetup pageSetup = worksheet.PageSetup;
            
            // Demonstriere die CenterHorizontally-Eigenschaft
            pageSetup.CenterHorizontally = true;
            pageSetup.PrintArea = "A1:B6";

            workbook.Save("CenterHorizontallyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


