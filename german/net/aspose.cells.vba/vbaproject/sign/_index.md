---
title: "VbaProject.Sign"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaProject-Methode. Signieren Sie dieses VBA-Projekt mit einer DigitalSignature"
type: docs
url: /de/net/aspose.cells.vba/vbaproject/sign/
---
## VbaProject.Sign method

Signiere dieses VBA-Projekt mit einer DigitalSignature

```csharp
public void Sign(DigitalSignature digitalSignature)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| digitalSignature | DigitalSignature | DigitalSignature |

### Beispiele

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
            // Laden Sie die Arbeitsmappe mit VBA-Projekt
            Workbook workbook = new Workbook("SignXlsm.xlsm");
            
            // Abrufen Sie das VBA-Projekt
            VbaProject vbaProject = workbook.VbaProject;
            
            if (vbaProject != null)
            {
                // Zertifikat aus Datei laden
                X509Certificate2 certificate = new X509Certificate2("YourCertificate.pfx", "password");
                
                // Erstellen Sie eine digitale Signatur
                DigitalSignature certSign = new DigitalSignature(certificate, "Test Signing", DateTime.Now);
                
                // Signieren Sie das VBA-Projekt
                vbaProject.Sign(certSign);
                
                // Das signierte Arbeitsbuch speichern
                using (MemoryStream stream = new MemoryStream())
                {
                    workbook.Save(stream, SaveFormat.Xlsm);
                    
                    // Überprüfen Sie die Signatur
                    Workbook verifyWorkbook = new Workbook(stream);
                    Console.WriteLine("Is Signed: " + verifyWorkbook.VbaProject.IsSigned);
                    Console.WriteLine("Is Valid Signed: " + verifyWorkbook.VbaProject.IsValidSigned);
                }
            }
        }
    }
}
```

### Siehe auch

* class [DigitalSignature](../../../aspose.cells.digitalsignatures/digitalsignature/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


