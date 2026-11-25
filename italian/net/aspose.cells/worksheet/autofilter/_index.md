---
title: "Worksheet.AutoFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Rappresenta il filtro automatico per il foglio di lavoro specificato"
type: docs
url: /it/net/aspose.cells/worksheet/autofilter/
---
## Worksheet.AutoFilter property

Rappresenta il filtro automatico per il foglio di lavoro specificato.

```csharp
public AutoFilter AutoFilter { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue("Electronics");
            worksheet.Cells["A3"].PutValue("Shirt");
            worksheet.Cells["B3"].PutValue("Clothing");
            worksheet.Cells["A4"].PutValue("Phone");
            worksheet.Cells["B4"].PutValue("Electronics");
            worksheet.Cells["A5"].PutValue("Pants");
            worksheet.Cells["B5"].PutValue("Clothing");

            // Applica filtro automatico
            worksheet.AutoFilter.Range = "A1:B5";
            worksheet.AutoFilter.Filter(1, "Electronics");

            // Aggiorna il filtro
            worksheet.AutoFilter.Refresh();

            // Salva la cartella di lavoro
            workbook.Save("AutoFilterDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [AutoFilter](../../autofilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


