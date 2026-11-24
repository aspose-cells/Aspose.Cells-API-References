---
title: "PageSetup.RightMargin"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt die Größe des rechten Randes in Zentimetern an."
type: docs
url: /de/net/aspose.cells/pagesetup/rightmargin/
---
## PageSetup.RightMargin property

Stellt die Größe des rechten Randes in Zentimetern dar.

```csharp
public double RightMargin { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyRightMarginDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Legen Sie unterschiedliche rechte Ränder fest und speichern Sie, um die Wirkung zu demonstrieren.
            worksheet.PageSetup.RightMargin = 0;
            workbook.Save("RightMargin_0.xlsx");

            worksheet.PageSetup.RightMargin = 1.0;
            workbook.Save("RightMargin_1.xlsx");

            worksheet.PageSetup.RightMargin = 2.5;
            workbook.Save("RightMargin_2.5.xlsx");

            // Geben Sie den aktuellen Wert des rechten Randes aus.
            Console.WriteLine("Current Right Margin: " + worksheet.PageSetup.RightMargin);
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


