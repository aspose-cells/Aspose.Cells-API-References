---
title: "OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OdsLoadOptions-Eigenschaft. Gibt an, ob der Standardstil von Excel auf den Hyperlink angewendet wird"
type: docs
url: /de/net/aspose.cells/odsloadoptions/applyexceldefaultstyletohyperlink/
---
## OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink property

Gibt an, ob der Standardstil von Excel auf Hyperlinks angewendet wird.

```csharp
public bool ApplyExcelDefaultStyleToHyperlink { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsLoadOptionsPropertyApplyExcelDefaultStyleToHyperlinkDemo
    {
        public static void Run()
        {
            // Eine Instanz von OdsLoadOptions erstellen
            OdsLoadOptions loadOptions = new OdsLoadOptions();

            // ApplyExcelDefaultStyleToHyperlink-Eigenschaft festlegen
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;

            // Eine ODS-Datei mit den angegebenen Optionen laden
            Workbook workbook = new Workbook("sample.ods", loadOptions);

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einen Hyperlink hinzu, um die Stil-Anwendung zu demonstrieren
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // Speichere die Arbeitsmappe in einer neuen Datei
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


