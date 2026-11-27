---
title: "Workbook.IsDigitallySigned"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Anger om detta kalkylblad är digitalt signerat"
type: docs
url: /sv/net/aspose.cells/workbook/isdigitallysigned/
---
## Workbook.IsDigitallySigned property

Anger om detta kalkylblad är digitalt signerat.

```csharp
public bool IsDigitallySigned { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsDigitallySignedDemo
    {
        public static void Run()
        {
            // Läs in en digitalt signerad Workbook
            Workbook book = new Workbook("Test_DigiSign.xlsx");
            
            // Kontrollera om arbetsboken är digitalt signerad
            bool isSigned = book.IsDigitallySigned;
            Console.WriteLine("Workbook is digitally signed: " + isSigned);

            if (isSigned)
            {
                // Spara en kopia (signaturen bevaras)
                book.Save("SignedCopy.xlsx");
                
                // Ta bort den digitala signaturen
                book.RemoveDigitalSignature();
                book.Save("UnsignedCopy.xlsx");
                
                // Verifiera att signaturen har tagits bort
                Workbook unsignedBook = new Workbook("UnsignedCopy.xlsx");
                Console.WriteLine("After removal, workbook is signed: " + unsignedBook.IsDigitallySigned);
            }
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


