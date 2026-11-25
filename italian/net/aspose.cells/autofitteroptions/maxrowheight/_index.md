---
title: "AutoFitterOptions.MaxRowHeight"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AutoFitterOptions. Ottiene e imposta l'altezza massima della riga in unità di Point quando si adattano automaticamente le righe"
type: docs
url: /it/net/aspose.cells/autofitteroptions/maxrowheight/
---
## AutoFitterOptions.MaxRowHeight property

Ottiene e imposta l'altezza massima della riga (in unità di Point) durante l'adattamento automatico delle righe.

```csharp
public double MaxRowHeight { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyMaxRowHeightDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta dati di esempio e formattazione
            worksheet.Cells["A1"].PutValue("This is a long text that will demonstrate row auto-fitting");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells.SetRowHeight(0, 10); // Set initial small row height

            // Crea AutoFitterOptions con l'impostazione MaxRowHeight
            AutoFitterOptions options = new AutoFitterOptions
            {
                MaxRowHeight = 50, // Limit maximum row height to 50 pixels
                OnlyAuto = true
            };

            // Adatta automaticamente la riga con limitazione dell'altezza
            worksheet.AutoFitRows(0, 0, options);

            Console.WriteLine("Row height after auto-fit with MaxRowHeight=50: " + worksheet.Cells.GetRowHeight(0));

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


