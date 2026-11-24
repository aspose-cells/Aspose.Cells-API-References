---
title: "DigitalSignature.SignTime"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DigitalSignature-Eigenschaft. Der Zeitpunkt, zu dem das Dokument signiert wurde"
type: docs
url: /de/net/aspose.cells.digitalsignatures/digitalsignature/signtime/
---
## DigitalSignature.SignTime property

Der Zeitpunkt, zu dem das Dokument signiert wurde.

```csharp
public DateTime SignTime { get; set; }
```

### Beispiele

```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertySignTimeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Digital Signature");

            // Erstelle und füge eine digitale Signatur hinzu
            try
            {
                X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
                DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
                
                DigitalSignatureCollection dsc = workbook.GetDigitalSignature();
                dsc.Add(signature);

                // Demonstriere die SignTime-Eigenschaft
                Console.WriteLine("Signature added at: " + signature.SignTime);

                // Das signierte Arbeitsbuch speichern
                workbook.Save("SignedWorkbook.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Siehe auch

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


