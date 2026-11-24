---
title: "Aufzählung OoxmlCompliance"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.OoxmlCompliance‑Enum. Ermöglicht die Angabe, welche OOXML‑Spezifikation beim Speichern im Xlsx‑Format verwendet wird."
type: docs
url: /de/net/aspose.cells/ooxmlcompliance/
---
## OoxmlCompliance enumeration

Ermöglicht die Angabe, welche OOXML-Spezifikation beim Speichern im Xlsx-Format verwendet wird.

```csharp
public enum OoxmlCompliance
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Ecma376_2006 | `0` | ECMA‑376 1. Auflage, 2006. |
| Iso29500_2008_Strict | `1` | ISO/IEC 29500:2008 Striktes Konformitätsniveau. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlComplianceDemo
    {
        public static void OoxmlComplianceExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Auf Arbeitsmappeneinstellungen zugreifen
            WorkbookSettings settings = workbook.Settings;

            // Setze das OOXML‑Konformitätsniveau auf ISO/IEC 29500:2008 Strikt
            settings.Compliance = OoxmlCompliance.Iso29500_2008_Strict;

            // Füge dem Arbeitsblatt einige Daten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, World!");

            // Speichere die Arbeitsmappe mit dem angegebenen OOXML‑Konformitätsniveau
            workbook.Save("OoxmlComplianceExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


