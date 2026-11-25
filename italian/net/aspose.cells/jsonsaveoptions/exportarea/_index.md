---
title: "JsonSaveOptions.ExportArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonSaveOptions. Ottiene o imposta l'intervallo di esportazione"
type: docs
url: /it/net/aspose.cells/jsonsaveoptions/exportarea/
---
## JsonSaveOptions.ExportArea property

Ottiene o imposta l'intervallo di esportazione.

```csharp
public CellArea ExportArea { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Riempi dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Configura le opzioni di salvataggio JSON con ExportArea
            JsonSaveOptions saveOptions = new JsonSaveOptions
            {
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 }
            };

            // Salva con l'area di esportazione specificata (A1:B3)
            workbook.Save("JsonExportAreaDemo.json", saveOptions);
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


