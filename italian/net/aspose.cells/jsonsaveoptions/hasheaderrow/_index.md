---
title: "JsonSaveOptions.HasHeaderRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonSaveOptions. Indica se l'intervallo contiene una riga di intestazione"
type: docs
url: /it/net/aspose.cells/jsonsaveoptions/hasheaderrow/
---
## JsonSaveOptions.HasHeaderRow property

Indica se l'intervallo contiene la riga di intestazione.

```csharp
public bool HasHeaderRow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi riga di intestazione
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            
            // Aggiungi righe di dati
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crea intervallo (A1:B3)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 2);

            // Esporta in JSON con HasHeaderRow = true (predefinito)
            JsonSaveOptions options1 = new JsonSaveOptions();
            options1.HasHeaderRow = true;
            string jsonWithHeaders = Aspose.Cells.Utility.JsonUtility.ExportRangeToJson(range, options1);
            Console.WriteLine("JSON with headers:\n" + jsonWithHeaders);

            // Esporta in JSON con HasHeaderRow = false
            JsonSaveOptions options2 = new JsonSaveOptions();
            options2.HasHeaderRow = false;
            string jsonWithoutHeaders = Aspose.Cells.Utility.JsonUtility.ExportRangeToJson(range, options2);
            Console.WriteLine("\nJSON without headers:\n" + jsonWithoutHeaders);
        }
    }
}
```

### Vedi anche

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


