---
title: "SpreadsheetML2003SaveOptions.IsIndentedFormatting"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Eigenschaft SpreadsheetML2003SaveOptions. Veranlasst, dass Kind-Elemente eingerückt werden"
type: docs
url: /de/net/aspose.cells/spreadsheetml2003saveoptions/isindentedformatting/
---
## SpreadsheetML2003SaveOptions.IsIndentedFormatting property

Veranlasst, dass Kind-Elemente eingerückt werden.

```csharp
public bool IsIndentedFormatting { get; set; }
```

### Hinweise

Der Standardwert ist true. Wenn der Wert false ist, reduziert dies die Größe der XML-Datei

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyIsIndentedFormattingDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);

            // Konfigurieren Sie Speicheroptionen mit eingerückter Formatierung
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions
            {
                IsIndentedFormatting = true
            };

            // Speichern mit eingerückter XML-Formatierung
            workbook.Save("output_indented.xml", saveOptions);

            // Speichern ohne eingerückte Formatierung zum Vergleich
            saveOptions.IsIndentedFormatting = false;
            workbook.Save("output_not_indented.xml", saveOptions);
        }
    }
}
```

### Siehe auch

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


