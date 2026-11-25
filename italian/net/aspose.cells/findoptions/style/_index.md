---
title: "FindOptions.Style"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FindOptions. Il formato da cercare"
type: docs
url: /it/net/aspose.cells/findoptions/style/
---
## FindOptions.Style property

Il formato da cercare.

```csharp
public Style Style { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea uno stile con carattere blu
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Blue;

            // Applica lo stile alla cella F2
            Cell cell = worksheet.Cells["F2"];
            cell.PutValue("SearchTarget");
            cell.SetStyle(style);

            // Crea le opzioni di ricerca con lo stile
            FindOptions options = new FindOptions();
            options.Style = style;

            // Trova la cella con lo stile corrispondente
            Cell foundCell = worksheet.Cells.Find(null, null, options);

            // Restituisci il nome della cella trovata
            Console.WriteLine("Cell found with matching style: " + foundCell?.Name);
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


