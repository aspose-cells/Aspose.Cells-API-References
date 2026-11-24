---
title: "XmlLoadOptions.DateFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XmlLoadOptions-Eigenschaft. Gibt das Datumsformat zurück und legt es fest"
type: docs
url: /de/net/aspose.cells/xmlloadoptions/dateformat/
---
## XmlLoadOptions.DateFormat property

Liest und setzt das Format des Datumswerts.

```csharp
public string DateFormat { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // Erstelle eine Instanz von XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Legen Sie das Datumsformat zum Parsen von Daten aus XML fest
            options.DateFormat = "yyyy-MM-dd";
            options.ConvertNumericOrDate = true;

            // Lade eine XML-Datei in ein Workbook mit den angegebenen Optionen
            Workbook workbook = new Workbook("input.xml", options);

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Zeigen Sie einige Zellen an, um die Datumsformatierung zu demonstrieren
            Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].Value);

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


