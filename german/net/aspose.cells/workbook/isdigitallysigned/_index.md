---
title: "Workbook.IsDigitallySigned"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Eigenschaft. Gibt an, ob diese Tabelle digital signiert ist"
type: docs
url: /de/net/aspose.cells/workbook/isdigitallysigned/
---
## Workbook.IsDigitallySigned property

Gibt an, ob diese Tabelle digital signiert ist.

```csharp
public bool IsDigitallySigned { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsDigitallySignedDemo
    {
        public static void Run()
        {
            // Ein digital signiertes Workbook laden
            Workbook book = new Workbook("Test_DigiSign.xlsx");
            
            // Prüfen, ob die Arbeitsmappe digital signiert ist
            bool isSigned = book.IsDigitallySigned;
            Console.WriteLine("Workbook is digitally signed: " + isSigned);

            if (isSigned)
            {
                // Eine Kopie speichern (Signatur bleibt erhalten)
                book.Save("SignedCopy.xlsx");
                
                // Die digitale Signatur entfernen
                book.RemoveDigitalSignature();
                book.Save("UnsignedCopy.xlsx");
                
                // Überprüfen, dass die Signatur entfernt wurde
                Workbook unsignedBook = new Workbook("UnsignedCopy.xlsx");
                Console.WriteLine("After removal, workbook is signed: " + unsignedBook.IsDigitallySigned);
            }
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


