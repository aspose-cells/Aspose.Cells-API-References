---
title: "CopyOptions.CopyInvalidFormulasAsValues"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CopyOptions. Se la formula non è valida per la destinazione, copia solo i valori"
type: docs
url: /it/net/aspose.cells/copyoptions/copyinvalidformulasasvalues/
---
## CopyOptions.CopyInvalidFormulasAsValues property

Se la formula non è valida per la destinazione, copia solo i valori.

```csharp
public bool CopyInvalidFormulasAsValues { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyCopyInvalidFormulasAsValuesDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di origine con un foglio di lavoro di esempio
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            
            // Aggiungi una formula che potrebbe essere non valida in alcuni contesti
            srcSheet.Cells["A1"].Formula = "=1/0"; // Division by zero - invalid formula
            srcSheet.Cells["A2"].Value = "Valid Data";

            // Crea una cartella di lavoro di destinazione
            Workbook destWorkbook = new Workbook();
            
            // Imposta le opzioni di copia per convertire le formule non valide in valori
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.CopyInvalidFormulasAsValues = true;

            // Copia il foglio di lavoro con le opzioni
            destWorkbook.Worksheets[0].Copy(srcSheet, copyOptions);

            // Verifica i risultati
            Console.WriteLine("A1 (invalid formula copied as value): " + 
                destWorkbook.Worksheets[0].Cells["A1"].Value); // Should show #DIV/0! as value
            Console.WriteLine("A2 (valid data): " + 
                destWorkbook.Worksheets[0].Cells["A2"].Value); // Should show "Valid Data"
        }
    }
}
```

### Vedi anche

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


