---
title: "VbaProject.Sign"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo VbaProject. Firma questo progetto VBA con una DigitalSignature"
type: docs
url: /it/net/aspose.cells.vba/vbaproject/sign/
---
## VbaProject.Sign method

Firma questo progetto VBA con una DigitalSignature

```csharp
public void Sign(DigitalSignature digitalSignature)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| digitalSignature | DigitalSignature | DigitalSignature |

### Esempi

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
            // Carica la cartella di lavoro con il progetto VBA
            Workbook workbook = new Workbook("SignXlsm.xlsm");
            
            // Ottieni il progetto VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            if (vbaProject != null)
            {
                // Carica il certificato da file
                X509Certificate2 certificate = new X509Certificate2("YourCertificate.pfx", "password");
                
                // Crea una firma digitale
                DigitalSignature certSign = new DigitalSignature(certificate, "Test Signing", DateTime.Now);
                
                // Firma il progetto VBA
                vbaProject.Sign(certSign);
                
                // Salva la cartella di lavoro firmata
                using (MemoryStream stream = new MemoryStream())
                {
                    workbook.Save(stream, SaveFormat.Xlsm);
                    
                    // Verifica la firma
                    Workbook verifyWorkbook = new Workbook(stream);
                    Console.WriteLine("Is Signed: " + verifyWorkbook.VbaProject.IsSigned);
                    Console.WriteLine("Is Valid Signed: " + verifyWorkbook.VbaProject.IsValidSigned);
                }
            }
        }
    }
}
```

### Vedi anche

* class [DigitalSignature](../../../aspose.cells.digitalsignatures/digitalsignature/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


