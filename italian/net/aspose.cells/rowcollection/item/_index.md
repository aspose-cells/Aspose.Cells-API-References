---
title: "RowCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RowCollection. Restituisce un oggetto Row dato l'indice di riga. L'oggetto Row dell'indice specificato verrà istanziato se non esiste già."
type: docs
url: /it/net/aspose.cells/rowcollection/item/
---
## RowCollection indexer

Restituisce un oggetto [`Row`](../../row/) dato l'indice di riga. L'oggetto Row dell'indice specificato verrà istanziato se non esiste già.

```csharp
public Row this[int rowIndex] { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta la larghezza standard per le colonne
            cells.StandardWidth = 20.0;

            // Accedi e formatta le righe usando la proprietà Item
            for (int i = 0; i < 5; i++)
            {
                Row row = cells.Rows[i]; // Using Item property
                Style rowStyle = workbook.CreateStyle();
                rowStyle.Font.IsBold = true;
                rowStyle.Font.Color = System.Drawing.Color.Blue;
                row.ApplyStyle(rowStyle, new StyleFlag { Font = true });
                
                // Accedi e formatta la cella nella riga
                Cell cell = cells[i, i]; // Using Cells indexer instead of row[i]
                cell.PutValue($"Row {i}, Col {i}");
                Style cellStyle = workbook.CreateStyle();
                cellStyle.BackgroundColor = System.Drawing.Color.LightYellow;
                cell.SetStyle(cellStyle);
            }

            // Salva la cartella di lavoro
            workbook.Save("RowCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


