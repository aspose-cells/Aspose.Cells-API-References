---
title: "Column.Width"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Column. Ottiene e imposta la larghezza della colonna in unità di caratteri"
type: docs
url: /it/net/aspose.cells/column/width/
---
## Column.Width property

Restituisce e imposta la larghezza della colonna in unità di caratteri.

```csharp
public double Width { get; set; }
```

### Osservazioni

Per i fogli di calcolo, la larghezza della colonna è misurata come il numero di caratteri della larghezza massima delle cifre dei numeri 0~9 così come visualizzate nel carattere dello stile normale.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyWidthDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta la larghezza per la colonna 3 (indice 2)
            worksheet.Cells.Columns[2].Width = 25.5;
            
            // Imposta la larghezza per la colonna 4 (indice 3)
            worksheet.Cells.Columns[3].Width = 40.0;
            
            // Ottieni e visualizza le larghezze
            Console.WriteLine("Column 3 Width: " + worksheet.Cells.Columns[2].Width);
            Console.WriteLine("Column 4 Width: " + worksheet.Cells.Columns[3].Width);
            
            // Salva la cartella di lavoro
            workbook.Save("ColumnWidthDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


