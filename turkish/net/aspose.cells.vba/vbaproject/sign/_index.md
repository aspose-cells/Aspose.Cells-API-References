---
title: "VbaProject.Sign"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaProject yöntemi. Bu VBA projesini bir DigitalSignature ile imzalayın"
type: docs
url: /tr/net/aspose.cells.vba/vbaproject/sign/
---
## VbaProject.Sign method

Bu VBA projesini bir DigitalSignature ile imzalar

```csharp
public void Sign(DigitalSignature digitalSignature)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| digitalSignature | DigitalSignature | DigitalSignature |

### Örnekler

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
            // VBA projesiyle birlikte çalışma kitabını yükleyin
            Workbook workbook = new Workbook("SignXlsm.xlsm");
            
            // VBA projesini alın
            VbaProject vbaProject = workbook.VbaProject;
            
            if (vbaProject != null)
            {
                // Dosyadan sertifika yükleyin
                X509Certificate2 certificate = new X509Certificate2("YourCertificate.pfx", "password");
                
                // Dijital imza oluşturun
                DigitalSignature certSign = new DigitalSignature(certificate, "Test Signing", DateTime.Now);
                
                // VBA projesini imzalayın
                vbaProject.Sign(certSign);
                
                // İmzalı çalışma kitabını kaydet
                using (MemoryStream stream = new MemoryStream())
                {
                    workbook.Save(stream, SaveFormat.Xlsm);
                    
                    // İmzayı doğrulayın
                    Workbook verifyWorkbook = new Workbook(stream);
                    Console.WriteLine("Is Signed: " + verifyWorkbook.VbaProject.IsSigned);
                    Console.WriteLine("Is Valid Signed: " + verifyWorkbook.VbaProject.IsValidSigned);
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [DigitalSignature](../../../aspose.cells.digitalsignatures/digitalsignature/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


