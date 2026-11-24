---
title: "PageSetup.IsPercentScale"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Wenn diese Eigenschaft False ist, steuern die Eigenschaften FitToPagesWide und FitToPagesTall, wie das Arbeitsblatt skaliert wird."
type: docs
url: /de/net/aspose.cells/pagesetup/ispercentscale/
---
## PageSetup.IsPercentScale property

Wenn diese Eigenschaft Falsch ist, steuern die Eigenschaften FitToPagesWide und FitToPagesTall, wie das Arbeitsblatt skaliert wird.

```csharp
public bool IsPercentScale { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsPercentScaleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greifen Sie auf PageSetup zu und setzen Sie die Skalierung auf 80 % (Prozentskala)
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.Zoom = 80;
            pageSetup.IsPercentScale = true;

            // Geben Sie die Einstellungen aus, um IsPercentScale zu demonstrieren
            Console.WriteLine("Zoom: " + pageSetup.Zoom);
            Console.WriteLine("IsPercentScale: " + pageSetup.IsPercentScale);

            // Speichere die Arbeitsmappe
            workbook.Save("PageSetup_IsPercentScale_Output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


