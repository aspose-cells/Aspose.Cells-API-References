---
title: "Workbook.RemoveDigitalSignature"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Tar bort digital signatur från detta kalkylblad"
type: docs
url: /sv/net/aspose.cells/workbook/removedigitalsignature/
---
## Workbook.RemoveDigitalSignature method

Tar bort digital signatur från detta kalkylblad.

```csharp
public void RemoveDigitalSignature()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveDigitalSignatureDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med digital signatur
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test Digital Signature");
            
            // Spara med digital signatur (i ett verkligt scenario skulle detta signeras externt)
            string signedPath = "SignedWorkbook.xlsx";
            book.Save(signedPath, SaveFormat.Xlsx);

            // Läs in den signerade arbetsboken
            Workbook signedBook = new Workbook(signedPath);
            Console.WriteLine("Workbook is digitally signed: " + signedBook.IsDigitallySigned);

            // Ta bort digital signatur
            signedBook.RemoveDigitalSignature();
            string unsignedPath = "UnsignedWorkbook.xlsx";
            signedBook.Save(unsignedPath);

            // Verifiera att signaturen har tagits bort
            Workbook unsignedBook = new Workbook(unsignedPath);
            Console.WriteLine("After removal, workbook is digitally signed: " + unsignedBook.IsDigitallySigned);
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


