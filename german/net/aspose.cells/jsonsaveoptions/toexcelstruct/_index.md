---
title: "JsonSaveOptions.ToExcelStruct"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "JsonSaveOptions-Eigenschaft. Gibt an, ob in eine JSON-Struktur der Excel-Datei konvertiert wird"
type: docs
url: /de/net/aspose.cells/jsonsaveoptions/toexcelstruct/
---
## JsonSaveOptions.ToExcelStruct property

Gibt an, ob in die JSON‑Struktur der Excel‑Datei konvertiert wird.

```csharp
public bool ToExcelStruct { get; set; }
```

### Hinweise

Nur für die Konvertierung eines Bereichs zu JSON.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyToExcelStructDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Einen Bereich zum Exportieren erstellen
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

            // JSON-Speicheroptionen mit ToExcelStruct konfigurieren
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ToExcelStruct = true;

            // Exportiere Bereich nach JSON
            string json = range.ToJson(saveOptions);
            Console.WriteLine(json);
        }
    }
}
```

### Siehe auch

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


