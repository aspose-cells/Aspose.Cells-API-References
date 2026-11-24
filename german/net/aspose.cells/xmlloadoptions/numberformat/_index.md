---
title: "XmlLoadOptions.NumberFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XmlLoadOptions-Eigenschaft. Gibt das Format des numerischen Werts zurück und legt es fest"
type: docs
url: /de/net/aspose.cells/xmlloadoptions/numberformat/
---
## XmlLoadOptions.NumberFormat property

Liest und setzt das Format des numerischen Werts.

```csharp
public string NumberFormat { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // Erstelle eine Instanz von XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Setzen Sie die NumberFormat-Eigenschaft, um Zahlen mit 2 Dezimalstellen anzuzeigen
            options.NumberFormat = "0.00";

            // Lade eine XML-Datei in ein Workbook mit den angegebenen Optionen
            Workbook workbook = new Workbook("input.xml", options);

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Legen Sie einige numerische Werte fest, um die Zahlenformatierung zu demonstrieren
            worksheet.Cells["A1"].PutValue(123);
            worksheet.Cells["A2"].PutValue(45.678);
            worksheet.Cells["A3"].PutValue(0.5);

            // Speichere die Arbeitsmappe in einer neuen Datei
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


