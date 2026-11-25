---
title: "Cells.MaxDisplayRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Ottiene l'intervallo massimo che include dati, celle unite e forme"
type: docs
url: /it/net/aspose.cells/cells/maxdisplayrange/
---
## Cells.MaxDisplayRange property

Ottiene l'intervallo massimo che include dati, celle unite e forme.

```csharp
public Range MaxDisplayRange { get; }
```

### Osservazioni

Restituisce null se il foglio di lavoro è vuoto a partire da Aspose.Cells 21.5.2.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxDisplayRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati alle celle per creare un intervallo di visualizzazione
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["B3"].PutValue(400);

            // Ottieni l'intervallo di visualizzazione massimo
            Aspose.Cells.Range maxDisplayRange = worksheet.Cells.MaxDisplayRange;

            // Emetti le informazioni dell'intervallo
            Console.WriteLine("Max Display Range:");
            Console.WriteLine($"Start Row: {maxDisplayRange.FirstRow}");
            Console.WriteLine($"Start Column: {maxDisplayRange.FirstColumn}");
            Console.WriteLine($"Total Rows: {maxDisplayRange.RowCount}");
            Console.WriteLine($"Total Columns: {maxDisplayRange.ColumnCount}");

            // Crea un nuovo intervallo basato sulle dimensioni dell'intervallo di visualizzazione massimo
            Aspose.Cells.Range customRange = worksheet.Cells.CreateRange(
                maxDisplayRange.FirstRow,
                maxDisplayRange.FirstColumn,
                maxDisplayRange.RowCount,
                maxDisplayRange.ColumnCount);

            // Applica la formattazione all'intervallo
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            style.Pattern = BackgroundType.Solid;
            customRange.ApplyStyle(style, new StyleFlag { FontBold = true, CellShading = true });

            // Salva la cartella di lavoro
            workbook.Save("MaxDisplayRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


