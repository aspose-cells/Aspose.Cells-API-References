---
title: "Cells.MaxDataRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Indice massimo della riga della cella che contiene dati"
type: docs
url: /it/net/aspose.cells/cells/maxdatarow/
---
## Cells.MaxDataRow property

Indice di riga massimo della cella che contiene dati.

```csharp
public int MaxDataRow { get; }
```

### Osservazioni

Restituisce -1 se non esiste alcuna cella che contiene dati. Questa proprietà deve iterare e controllare celle e righe dinamicamente, quindi è un processo dispendioso in termini di tempo e non dovrebbe essere invocata ripetutamente, ad esempio usandola direttamente come condizione in un ciclo.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxDataRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["B4"].PutValue(30);

            // Dimostrare l'uso di MaxDataRow
            int maxRow = sheet.Cells.MaxDataRow;
            Console.WriteLine("Max data row: " + maxRow);

            // Crea un'area di celle usando MaxDataRow
            int startRow = 0;
            int startColumn = 0;
            int endRow = sheet.Cells.MaxDataRow;
            int endColumn = sheet.Cells.MaxDataColumn;

            // Applica la formattazione all'intervallo di dati
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            
            // Applica lo stile all'intervallo
            sheet.Cells.CreateRange(startRow, startColumn, endRow + 1, endColumn + 1).ApplyStyle(style, new StyleFlag { FontBold = true });

            // Salva la cartella di lavoro
            workbook.Save("MaxDataRowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


