---
title: "PageSetup.SetHeader"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Methode. Legt ein Skript fest, das die Kopfzeile einer Excel-Datei formatiert"
type: docs
url: /de/net/aspose.cells/pagesetup/setheader/
---
## PageSetup.SetHeader method

Legt ein Skript fest, das die Kopfzeile einer Excel-Datei formatiert.

```csharp
public void SetHeader(int section, string headerScript)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | Int32 | 0: Linker Abschnitt, 1: Mittlerer Abschnitt, 2: Rechter Abschnitt. |
| headerScript | String | Kopfzeilenformat‑Skript. |

### Hinweise

Skriptbefehle:

| **Command** | **Beschreibung** |
| --- | --- |
| &amp;P | Aktuelle Seitenzahl |
| &amp;N | Seitenanzahl |
| &amp;D | Aktuelles Datum |
| &amp;T | Aktuelle Uhrzeit |
| &amp;A | Blattname |
| &amp;F | Dateiname ohne Pfad |
| &amp;"&lt;FontName&gt;" | Schriftname, zum Beispiel: &amp;"Arial" |
| &amp;"&lt;FontName&gt;, &lt;FontStyle&gt;" | Schriftname und Schriftstil, zum Beispiel: &amp;"Arial,Bold" |
| &amp;&lt;FontSize&gt; | Schriftgröße. Wenn diesem Befehl eine einfache Zahl folgt, die in der Kopfzeile gedruckt werden soll, wird sie durch ein Leerzeichen von der Schrifthöhe getrennt. |
| &amp;K&lt;RRGGBB&gt; | Schriftfarbe, zum Beispiel (ROT): &amp;KFF0000 |
| &amp;G | Bildskript |

Zum Beispiel: "&amp;Arial,Bold&amp;8Header Note"

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Verschiedene Kopfzeilenabschnitte mit verschiedenen Befehlen festlegen
            pageSetup.SetHeader(0, "&F"); // Left section - File name
            pageSetup.SetHeader(1, "Page &P of &N"); // Center section - Page numbering
            pageSetup.SetHeader(2, "&D"); // Right section - Date

            workbook.Save("PageSetup_SetHeader_Example.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


