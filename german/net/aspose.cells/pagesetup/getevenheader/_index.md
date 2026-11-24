---
title: "PageSetup.GetEvenHeader"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Methode. Ruft ein Skript ab, das die gerade Kopfzeile einer Excel-Datei formatiert"
type: docs
url: /de/net/aspose.cells/pagesetup/getevenheader/
---
## PageSetup.GetEvenHeader method

Ruft ein Skript ab, das die gerade Kopfzeile einer Excel-Datei formatiert.

```csharp
public string GetEvenHeader(int section)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | Int32 | 0: Linker Abschnitt, 1: Mittlerer Abschnitt, 2: Rechter Abschnitt. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetEvenHeaderWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Unterschiedliche ungerade und gerade Seitenkopf- und -fußzeilen aktivieren
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.IsHFDiffOddEven = true;
            
            // Gerade Seitenkopfzeile festlegen
            pageSetup.SetEvenHeader(0, "&CEven Page Header Center");
            pageSetup.SetEvenHeader(1, "&LEven Page Header Left");
            pageSetup.SetEvenHeader(2, "&REven Page Header Right");
            
            // Gerade Seitenkopfzeilen abrufen und ausgeben
            Console.WriteLine("Even Header Center: " + pageSetup.GetEvenHeader(0));
            Console.WriteLine("Even Header Left: " + pageSetup.GetEvenHeader(1));
            Console.WriteLine("Even Header Right: " + pageSetup.GetEvenHeader(2));
            
            // Speichere die Arbeitsmappe
            workbook.Save("PageSetup_GetEvenHeaderDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


