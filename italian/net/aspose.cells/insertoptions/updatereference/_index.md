---
title: "InsertOptions.UpdateReference"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà InsertOptions. Indica se i riferimenti in altri fogli di lavoro verranno aggiornati"
type: docs
url: /it/net/aspose.cells/insertoptions/updatereference/
---
## InsertOptions.UpdateReference property

Indica se i riferimenti in altri fogli di lavoro verranno aggiornati.

```csharp
public bool UpdateReference { get; set; }
```

### Osservazioni

A partire dalla versione 26.7 impostiamo il valore predefinito di questa proprietà a true.

### Esempi

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class InsertOptionsPropertyUpdateReferenceDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook wb = new Workbook();
            
            // Aggiungi un secondo foglio di lavoro e imposta le formule che fanno riferimento a Sheet1
            Worksheet sheet2 = wb.Worksheets.Add("Sheet2");
            sheet2.Cells["A1"].Formula = "=Sheet1!A10";
            sheet2.Cells["B1"].Formula = "=Sheet1!A5";
            
            // Imposta le formule in Sheet1
            Worksheet sheet1 = wb.Worksheets[0];
            sheet1.Cells["A1"].Formula = "=A10";
            sheet1.Cells["B1"].Formula = "=A5";

            // Crea le opzioni di inserimento con UpdateReference abilitato
            InsertOptions iopts = new InsertOptions();
            iopts.UpdateReference = true;
            
            // Traccia le modifiche delle formule
            HashSet<string> changedCells = new HashSet<string>();
            iopts.UpdateReference = true;
            
            // Inserisci righe che aggiorneranno i riferimenti nelle formule
            sheet1.Cells.InsertRows(5, 3, iopts);
            
            // Restituisci il conteggio delle celle modificate
            Console.WriteLine("Formulas were automatically updated due to UpdateReference=true");
            
            // Visualizza le formule aggiornate
            Console.WriteLine("Sheet1 A1 formula: " + sheet1.Cells["A1"].Formula);
            Console.WriteLine("Sheet2 A1 formula: " + sheet2.Cells["A1"].Formula);
        }
    }
}
```

### Vedi anche

* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


