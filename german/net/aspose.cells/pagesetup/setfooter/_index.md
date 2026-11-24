---
title: "PageSetup.SetFooter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup‑Methode. Legt ein Skript fest, das die Fußzeile einer Excel‑Datei formatiert."
type: docs
url: /de/net/aspose.cells/pagesetup/setfooter/
---
## PageSetup.SetFooter method

Legt ein Skript fest, das die Fußzeile einer Excel-Datei formatiert.

```csharp
public void SetFooter(int section, string footerScript)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | Int32 | 0: Linker Abschnitt, 1: Mittlerer Abschnitt, 2: Rechter Abschnitt. |
| footerScript | String | Fußzeilenformatierungs‑Skript. |

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

Zum Beispiel: "&amp;Arial,Bold&amp;8Footer Note"

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFooterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.PageSetup.SetFooter(0, "Page &P");
            worksheet.PageSetup.SetFooter(1, "&D");
            worksheet.PageSetup.SetFooter(2, "&A");
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


