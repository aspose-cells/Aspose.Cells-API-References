---
title: "Workbook.IsDigitallySigned"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Workbook. Indica se questo foglio di calcolo è firmato digitalmente"
type: docs
url: /it/net/aspose.cells/workbook/isdigitallysigned/
---
## Workbook.IsDigitallySigned property

Indica se questo foglio di calcolo è firmato digitalmente.

```csharp
public bool IsDigitallySigned { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsDigitallySignedDemo
    {
        public static void Run()
        {
            // Carica un workbook firmato digitalmente
            Workbook book = new Workbook("Test_DigiSign.xlsx");
            
            // Verifica se la cartella di lavoro è firmata digitalmente
            bool isSigned = book.IsDigitallySigned;
            Console.WriteLine("Workbook is digitally signed: " + isSigned);

            if (isSigned)
            {
                // Salva una copia (la firma verrà preservata)
                book.Save("SignedCopy.xlsx");
                
                // Rimuovi la firma digitale
                book.RemoveDigitalSignature();
                book.Save("UnsignedCopy.xlsx");
                
                // Verifica che la firma sia stata rimossa
                Workbook unsignedBook = new Workbook("UnsignedCopy.xlsx");
                Console.WriteLine("After removal, workbook is signed: " + unsignedBook.IsDigitallySigned);
            }
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


