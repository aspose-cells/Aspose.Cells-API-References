---
title: "PageSetup.SetFirstPageHeader"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Methode. Legt ein Skript fest, das die erste Seitenkopfzeile einer Excel-Datei formatiert. Wirkt nur in Excel 2007, wenn IsHFDiffFirst true ist."
type: docs
url: /de/net/aspose.cells/pagesetup/setfirstpageheader/
---
## PageSetup.SetFirstPageHeader method

Legt ein Skript fest, das die Kopfzeile der ersten Seite einer Excel-Datei formatiert. Wirkt nur in Excel 2007, wenn IsHFDiffFirst true ist.

```csharp
public void SetFirstPageHeader(int section, string headerScript)
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
    public class PageSetupMethodSetFirstPageHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Setze die erste Seitenkopfzeile mit Abschnittsnummer und Kopfzeilentext
            pageSetup.SetFirstPageHeader(2, "&CHeader Text");

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


