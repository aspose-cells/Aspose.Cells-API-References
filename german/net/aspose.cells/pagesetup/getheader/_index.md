---
title: "PageSetup.GetHeader"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Methode. Ruft ein Skript ab, das den Header einer Excel-Datei formatiert"
type: docs
url: /de/net/aspose.cells/pagesetup/getheader/
---
## PageSetup.GetHeader method

Ruft ein Skript ab, das die Kopfzeile einer Excel-Datei formatiert.

```csharp
public string GetHeader(int section)
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
    public class PageSetupMethodGetHeaderWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setzen Sie den Header für Abschnitt 2
            worksheet.PageSetup.SetHeader(2, "&8Report ID: TEST01\n你好Public");
            
            // Rufen Sie den Header für Abschnitt 2 ab und geben Sie ihn aus
            string header = worksheet.PageSetup.GetHeader(2);
            Console.WriteLine("Header for section 2: " + header);
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


