---
title: "JsonSaveOptions.HasHeaderRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "JsonSaveOptions-Eigenschaft. Gibt an, ob der Bereich eine Kopfzeile enthält"
type: docs
url: /de/net/aspose.cells/jsonsaveoptions/hasheaderrow/
---
## JsonSaveOptions.HasHeaderRow property

Gibt an, ob der Bereich eine Kopfzeilenzeile enthält.

```csharp
public bool HasHeaderRow { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Kopfzeile hinzufügen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            
            // Datenzeilen hinzufügen
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Bereich erstellen (A1:B3)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 2);

            // Exportieren nach JSON mit HasHeaderRow = true (Standard)
            JsonSaveOptions options1 = new JsonSaveOptions();
            options1.HasHeaderRow = true;
            string jsonWithHeaders = Aspose.Cells.Utility.JsonUtility.ExportRangeToJson(range, options1);
            Console.WriteLine("JSON with headers:\n" + jsonWithHeaders);

            // Exportieren nach JSON mit HasHeaderRow = false
            JsonSaveOptions options2 = new JsonSaveOptions();
            options2.HasHeaderRow = false;
            string jsonWithoutHeaders = Aspose.Cells.Utility.JsonUtility.ExportRangeToJson(range, options2);
            Console.WriteLine("\nJSON without headers:\n" + jsonWithoutHeaders);
        }
    }
}
```

### Siehe auch

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


