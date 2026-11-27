---
title: "VbaProject.Sign"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProject-metod. Signera detta VBA-projekt med en DigitalSignature"
type: docs
url: /sv/net/aspose.cells.vba/vbaproject/sign/
---
## VbaProject.Sign method

Signera detta VBA-projekt med en DigitalSignature

```csharp
public void Sign(DigitalSignature digitalSignature)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| digitalSignature | DigitalSignature | DigitalSignature |

### Exempel

```csharp
using System;
using System.IO;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.Vba;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class VbaProjectMethodSignWithDigitalSignatureDemo
    {
        public static void Run()
        {
            // Läs in arbetsboken med VBA-projektet
            Workbook workbook = new Workbook("SignXlsm.xlsm");
            
            // Hämta VBA-projektet
            VbaProject vbaProject = workbook.VbaProject;
            
            if (vbaProject != null)
            {
                // Läs in certifikat från fil
                X509Certificate2 certificate = new X509Certificate2("YourCertificate.pfx", "password");
                
                // Skapa en digital signatur
                DigitalSignature certSign = new DigitalSignature(certificate, "Test Signing", DateTime.Now);
                
                // Signera VBA-projektet
                vbaProject.Sign(certSign);
                
                // Spara den signerade arbetsboken
                using (MemoryStream stream = new MemoryStream())
                {
                    workbook.Save(stream, SaveFormat.Xlsm);
                    
                    // Verifiera signaturen
                    Workbook verifyWorkbook = new Workbook(stream);
                    Console.WriteLine("Is Signed: " + verifyWorkbook.VbaProject.IsSigned);
                    Console.WriteLine("Is Valid Signed: " + verifyWorkbook.VbaProject.IsValidSigned);
                }
            }
        }
    }
}
```

### Se även

* class [DigitalSignature](../../../aspose.cells.digitalsignatures/digitalsignature/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


