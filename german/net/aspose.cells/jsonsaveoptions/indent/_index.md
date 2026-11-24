---
title: "JsonSaveOptions.Indent"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "JsonSaveOptions-Eigenschaft. Gibt die Einrückung an"
type: docs
url: /de/net/aspose.cells/jsonsaveoptions/indent/
---
## JsonSaveOptions.Indent property

Gibt die Einrückung an.

```csharp
public string Indent { get; set; }
```

### Hinweise

Wenn die Einrückung null oder leer ist, wird das exportierte JSON nicht formatiert.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyIndentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // JSON-Speicheroptionen mit Einrückung konfigurieren
            JsonSaveOptions saveOptions = new JsonSaveOptions
            {
                Indent = "    ", // 4 spaces for indentation
                ExportArea = new CellArea { StartRow = 0, EndRow = 3, StartColumn = 0, EndColumn = 1 },
                HasHeaderRow = true
            };

            // Mit eingerückter JSON-Ausgabe speichern
            workbook.Save("IndentedJsonOutput.json", saveOptions);
        }
    }
}
```

### Siehe auch

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


