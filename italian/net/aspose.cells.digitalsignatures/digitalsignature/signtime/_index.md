---
title: "DigitalSignature.SignTime"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DigitalSignature. Il momento in cui il documento è stato firmato"
type: docs
url: /it/net/aspose.cells.digitalsignatures/digitalsignature/signtime/
---
## DigitalSignature.SignTime property

Il tempo in cui il documento è stato firmato.

```csharp
public DateTime SignTime { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Digital Signature");

            // Crea e aggiungi una firma digitale
            try
            {
                X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
                DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
                
                DigitalSignatureCollection dsc = workbook.GetDigitalSignature();
                dsc.Add(signature);

                // Dimostra la proprietà SignTime
                Console.WriteLine("Signature added at: " + signature.SignTime);

                // Salva la cartella di lavoro firmata
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

### Vedi anche

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


