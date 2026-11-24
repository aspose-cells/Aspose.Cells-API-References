---
title: "PageSetup.IsHFAlignMargins"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt an, ob Kopf- und Fußzeilenränder mit den Seitenrändern ausgerichtet sind. Wenn diese Eigenschaft true ist, werden die linke Kopf- und Fußzeile mit dem linken Rand und die rechte Kopf- und Fußzeile mit dem rechten Rand ausgerichtet. Diese Option ist standardmäßig aktiviert."
type: docs
url: /de/net/aspose.cells/pagesetup/ishfalignmargins/
---
## PageSetup.IsHFAlignMargins property

Gibt an, ob Kopf- und Fußzeilenränder mit den Seitenrändern ausgerichtet sind. Ist diese Eigenschaft wahr, werden die linke Kopf- und Fußzeile mit dem linken Rand und die rechte Kopf- und Fußzeile mit dem rechten Rand ausgerichtet. Diese Option ist standardmäßig aktiviert.

```csharp
public bool IsHFAlignMargins { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFAlignMarginsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greifen Sie auf das PageSetup zu.
            PageSetup pageSetup = worksheet.PageSetup;

            // Setzen Sie IsHFAlignMargins auf true.
            pageSetup.IsHFAlignMargins = true;
            Console.WriteLine("IsHFAlignMargins set to: " + pageSetup.IsHFAlignMargins);

            // Ändern Sie IsHFAlignMargins auf false
            pageSetup.IsHFAlignMargins = false;
            Console.WriteLine("IsHFAlignMargins changed to: " + pageSetup.IsHFAlignMargins);

            // Speichere die Arbeitsmappe
            workbook.Save("PageSetup_IsHFAlignMargins_Example.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


