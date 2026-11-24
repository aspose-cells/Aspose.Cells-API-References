---
title: "PageSetup.SetEvenHeader"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Methode. Legt ein Skript fest, das die gerade Seitenkopfzeile einer Excel-Datei formatiert. Wirkt nur in Excel 2007, wenn IsHFDiffOddEven true ist."
type: docs
url: /de/net/aspose.cells/pagesetup/setevenheader/
---
## PageSetup.SetEvenHeader method

Legt ein Skript fest, das die gerade Seitenkopfzeile einer Excel-Datei formatiert. Wirkt nur in Excel 2007, wenn IsHFDiffOddEven true ist.

```csharp
public void SetEvenHeader(int section, string headerScript)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | Int32 | 0: Linker Abschnitt, 1: Mittlerer Abschnitt, 2: Rechter Abschnitt. |
| headerScript | String | Kopfzeilenformat‑Skript. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetEvenHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Aktiviere unterschiedliche Kopf‑/Fußzeilen für ungerade und gerade Seiten
            pageSetup.IsHFDiffOddEven = true;

            // Setze die gerade Seitenkopfzeile mit Abschnittsindex und Text
            pageSetup.SetEvenHeader(1, "Even Page Header - Center Section");
            pageSetup.SetEvenHeader(0, "Even Page Header - Left Section");
            pageSetup.SetEvenHeader(2, "Even Page Header - Right Section");

            // Speichere die Arbeitsmappe
            workbook.Save("PageSetup_SetEvenHeaderExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


