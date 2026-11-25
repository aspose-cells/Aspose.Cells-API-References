---
title: "PaginatedSaveOptions.GridlineType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PaginatedSaveOptions. Ottiene o imposta il tipo di linea della griglia"
type: docs
url: /it/net/aspose.cells/paginatedsaveoptions/gridlinetype/
---
## PaginatedSaveOptions.GridlineType property

Ottiene o imposta il tipo di griglia.

```csharp
public GridlineType GridlineType { get; set; }
```

### Osservazioni

Il valore predefinito è il tipo Dotted.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyGridlineTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio e abilita le linee della griglia
            worksheet.Cells["A1"].PutValue("GridlineType Demo");
            worksheet.Cells["B2"].PutValue(1);
            worksheet.Cells["C3"].PutValue(2);
            worksheet.Cells["D4"].PutValue(3);
            worksheet.IsGridlinesVisible = true;

            // Crea le opzioni di salvataggio PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Dimostra la proprietà GridlineType
            pdfSaveOptions.GridlineType = GridlineType.Dotted;

            // Salva la cartella di lavoro con le linee della griglia
            workbook.Save("GridlineTypeDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Vedi anche

* enum [GridlineType](../../gridlinetype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


