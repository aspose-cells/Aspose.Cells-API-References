---
title: "JsonSaveOptions.ToExcelStruct"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonSaveOptions. Indica se convertire in struttura JSON del file Excel"
type: docs
url: /it/net/aspose.cells/jsonsaveoptions/toexcelstruct/
---
## JsonSaveOptions.ToExcelStruct property

Indica se convertire in una struttura JSON del file Excel.

```csharp
public bool ToExcelStruct { get; set; }
```

### Osservazioni

Solo per convertire l'intervallo in JSON.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyToExcelStructDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Crea un intervallo da esportare
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

            // Configura le opzioni di salvataggio JSON con ToExcelStruct
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ToExcelStruct = true;

            // Esporta intervallo in JSON
            string json = range.ToJson(saveOptions);
            Console.WriteLine(json);
        }
    }
}
```

### Vedi anche

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


