---
title: "Workbook.RemoveDigitalSignature"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Rimuove la firma digitale da questo foglio di calcolo"
type: docs
url: /it/net/aspose.cells/workbook/removedigitalsignature/
---
## Workbook.RemoveDigitalSignature method

Rimuove la firma digitale da questo foglio di calcolo.

```csharp
public void RemoveDigitalSignature()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveDigitalSignatureDemo
    {
        public static void Run()
        {
            // Crea un workbook con firma digitale
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test Digital Signature");
            
            // Salva con firma digitale (in uno scenario reale questo sarebbe firmato esternamente)
            string signedPath = "SignedWorkbook.xlsx";
            book.Save(signedPath, SaveFormat.Xlsx);

            // Carica il workbook firmato
            Workbook signedBook = new Workbook(signedPath);
            Console.WriteLine("Workbook is digitally signed: " + signedBook.IsDigitallySigned);

            // Rimuovi firma digitale
            signedBook.RemoveDigitalSignature();
            string unsignedPath = "UnsignedWorkbook.xlsx";
            signedBook.Save(unsignedPath);

            // Verifica che la firma sia stata rimossa
            Workbook unsignedBook = new Workbook(unsignedPath);
            Console.WriteLine("After removal, workbook is digitally signed: " + unsignedBook.IsDigitallySigned);
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


