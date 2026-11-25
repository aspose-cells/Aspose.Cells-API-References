---
title: "Cells.PreserveString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Ottiene o imposta un valore che indica se tutti i valori del foglio di lavoro sono conservati come stringhe. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/cells/preservestring/
---
## Cells.PreserveString property

Ottiene o imposta un valore che indica se tutti i valori del foglio di lavoro sono conservati come stringhe. Il valore predefinito è false.

```csharp
public bool PreserveString { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyPreserveStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta la proprietà PreserveString su true
            cells.PreserveString = true;

            // Aggiungi valori stringa alle celle
            cells["A1"].PutValue("Preserved String 1");
            cells["B1"].PutValue("Preserved String 2");

            // Accedi ai valori (verranno conservati come stringhe)
            Console.WriteLine("Cell A1 value: " + cells["A1"].StringValue);
            Console.WriteLine("Cell B1 value: " + cells["B1"].StringValue);

            // Salva la cartella di lavoro
            workbook.Save("PreserveStringDemo.xlsx", SaveFormat.Xlsx);

            // Carica la cartella di lavoro salvata per verificare la conservazione
            Workbook loadedWorkbook = new Workbook("PreserveStringDemo.xlsx");
            Cells loadedCells = loadedWorkbook.Worksheets[0].Cells;

            // Stampa i valori conservati
            Console.WriteLine("\nAfter loading:");
            Console.WriteLine("Cell A1 value: " + loadedCells["A1"].StringValue);
            Console.WriteLine("Cell B1 value: " + loadedCells["B1"].StringValue);

            // Dimostra il confronto della proprietà PreserveString
            Console.WriteLine("\nPreserveString property matches: " + 
                (cells.PreserveString == loadedCells.PreserveString));
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


