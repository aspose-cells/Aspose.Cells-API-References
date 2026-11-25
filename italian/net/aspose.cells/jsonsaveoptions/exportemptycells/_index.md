---
title: "JsonSaveOptions.ExportEmptyCells"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonSaveOptions. Indica se esportare le celle vuote come null"
type: docs
url: /it/net/aspose.cells/jsonsaveoptions/exportemptycells/
---
## JsonSaveOptions.ExportEmptyCells property

Indica se esportare le celle vuote come null.

```csharp
public bool ExportEmptyCells { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportEmptyCellsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Riempi i dati con alcune celle vuote
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue(2.99); // B2 is intentionally left empty

            // Crea JsonSaveOptions con ExportEmptyCells impostato su false
            JsonSaveOptions options = new JsonSaveOptions
            {
                ExportEmptyCells = false
            };

            // Salva in JSON - le celle vuote saranno ignorate
            workbook.Save("output_skip_empty.json", options);

            // Cambia ExportEmptyCells a true
            options.ExportEmptyCells = true;

            // Salva di nuovo - le celle vuote saranno incluse
            workbook.Save("output_include_empty.json", options);
        }
    }
}
```

### Vedi anche

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


