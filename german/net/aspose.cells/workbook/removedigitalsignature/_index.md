---
title: "Workbook.RemoveDigitalSignature"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Entfernt die digitale Signatur aus diesem Tabellenblatt"
type: docs
url: /de/net/aspose.cells/workbook/removedigitalsignature/
---
## Workbook.RemoveDigitalSignature method

Entfernt die digitale Signatur aus diesem Tabellenblatt.

```csharp
public void RemoveDigitalSignature()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveDigitalSignatureDemo
    {
        public static void Run()
        {
            // Ein Arbeitsbuch mit digitaler Signatur erstellen
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test Digital Signature");
            
            // Mit digitaler Signatur speichern (in einem realen Szenario würde dies extern signiert werden)
            string signedPath = "SignedWorkbook.xlsx";
            book.Save(signedPath, SaveFormat.Xlsx);

            // Das signierte Arbeitsbuch laden
            Workbook signedBook = new Workbook(signedPath);
            Console.WriteLine("Workbook is digitally signed: " + signedBook.IsDigitallySigned);

            // Digitale Signatur entfernen
            signedBook.RemoveDigitalSignature();
            string unsignedPath = "UnsignedWorkbook.xlsx";
            signedBook.Save(unsignedPath);

            // Überprüfen, dass die Signatur entfernt wurde
            Workbook unsignedBook = new Workbook(unsignedPath);
            Console.WriteLine("After removal, workbook is digitally signed: " + unsignedBook.IsDigitallySigned);
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


