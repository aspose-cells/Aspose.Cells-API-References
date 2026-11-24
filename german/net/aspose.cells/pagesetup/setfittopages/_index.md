---
title: "PageSetup.SetFitToPages"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Methode. Legt die Anzahl der Seiten fest, auf die das Arbeitsblatt beim Drucken skaliert wird"
type: docs
url: /de/net/aspose.cells/pagesetup/setfittopages/
---
## PageSetup.SetFitToPages method

Legt die Anzahl der Seiten fest, auf die das Arbeitsblatt beim Drucken skaliert wird.

```csharp
public void SetFitToPages(int wide, int tall)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| breit | Int32 | Seiten breit. |
| hoch | Int32 | Seiten hoch. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFitToPagesWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf das PageSetup des ersten Arbeitsblatts zu.
            PageSetup setup = workbook.Worksheets[0].PageSetup;
            
            // Fit-to-Pages-Einstellungen festlegen
            setup.SetFitToPages(2, 3);
            
            // Einstellungen überprüfen und ausgeben
            Console.WriteLine("IsPercentScale: " + setup.IsPercentScale);
            Console.WriteLine("FitToPagesWide: " + setup.FitToPagesWide);
            Console.WriteLine("FitToPagesTall: " + setup.FitToPagesTall);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


