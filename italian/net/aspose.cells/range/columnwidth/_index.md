---
title: "Range.ColumnWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Range. Imposta o ottiene la larghezza della colonna di questo intervallo"
type: docs
url: /it/net/aspose.cells/range/columnwidth/
---
## Range.ColumnWidth property

Imposta o ottiene la larghezza della colonna di questo intervallo

```csharp
public double ColumnWidth { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangePropertyColumnWidthDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi a un intervallo (colonne B a D)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B:D");
            
            // Visualizza la larghezza corrente della colonna
            Console.WriteLine("Current ColumnWidth: " + range.ColumnWidth);

            // Imposta una nuova larghezza della colonna (in unità di carattere)
            range.ColumnWidth = 15.0;

            // Popola le celle per dimostrare l'effetto
            worksheet.Cells["B1"].PutValue("This is column B");
            worksheet.Cells["C1"].PutValue("This is column C");
            worksheet.Cells["D1"].PutValue("This is column D");

            // Adatta automaticamente le righe per mostrare il contenuto
            worksheet.AutoFitRows();

            // Salva la cartella di lavoro
            workbook.Save("ColumnWidthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


