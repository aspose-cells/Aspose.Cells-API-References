---
title: "DigitalSignature.SignTime"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DigitalSignature-egenskap. Tiden då dokumentet signerades"
type: docs
url: /sv/net/aspose.cells.digitalsignatures/digitalsignature/signtime/
---
## DigitalSignature.SignTime property

Tidpunkten då dokumentet signerades.

```csharp
public DateTime SignTime { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Digital Signature");

            // Skapa och lägg till en digital signatur
            try
            {
                X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
                DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
                
                DigitalSignatureCollection dsc = workbook.GetDigitalSignature();
                dsc.Add(signature);

                // Demonstrera SignTime-egenskapen
                Console.WriteLine("Signature added at: " + signature.SignTime);

                // Spara den signerade arbetsboken
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

### Se även

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


