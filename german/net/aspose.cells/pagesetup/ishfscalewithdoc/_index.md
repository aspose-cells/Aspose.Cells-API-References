---
title: "PageSetup.IsHFScaleWithDoc"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup‑Eigenschaft. Gibt an, ob Kopf‑ und Fußzeile mit der Dokumentskalierung skaliert werden. Gilt nur für Excel 2007"
type: docs
url: /de/net/aspose.cells/pagesetup/ishfscalewithdoc/
---
## PageSetup.IsHFScaleWithDoc property

Gibt an, ob Kopf- und Fußzeile mit der Dokumentskalierung skaliert werden. Gilt nur für Excel 2007.

```csharp
public bool IsHFScaleWithDoc { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFScaleWithDocDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Zugriff auf PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Grundlegende PageSetup festlegen
            pageSetup.Orientation = PageOrientationType.Landscape;
            pageSetup.PaperSize = PaperSizeType.PaperA4;

            // Demonstration der IsHFScaleWithDoc‑Eigenschaft
            pageSetup.IsHFScaleWithDoc = true;
            Console.WriteLine("Header/Footer scaling with document is set to: " + pageSetup.IsHFScaleWithDoc);

            // Speichere die Arbeitsmappe
            workbook.Save("PageSetup_IsHFScaleWithDoc_Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


