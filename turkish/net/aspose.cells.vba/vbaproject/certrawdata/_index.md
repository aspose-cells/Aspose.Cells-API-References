---
title: "VbaProject.CertRawData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaProject özelliği. Bu VBA projesi imzalıysa sertifika ham verilerini alır"
type: docs
url: /tr/net/aspose.cells.vba/vbaproject/certrawdata/
---
## VbaProject.CertRawData property

Bu VBA projesi imzalıysa sertifikanın ham verisini alır.

```csharp
public byte[] CertRawData { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;
    using System.IO;

    public class VbaProjectPropertyCertRawDataDemo
    {
        public static void Run()
        {
            // VBA projesi içeren yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            // Workbook zaten bir VbaProject içerdiği için yeni bir VbaProject oluşturmanıza gerek yok

            // VBA projesine eriş
            VbaProject vbaProject = workbook.VbaProject;

            // VBA projesinin imzalı olup olmadığını kontrol edin
            if (vbaProject.IsSigned)
            {
                // İmzalıysa sertifika ham verilerini göster
                byte[] certData = vbaProject.CertRawData;
                Console.WriteLine("VBA Project is signed. Certificate raw data length: " + (certData != null ? certData.Length : 0));

                // Örnek: Sertifika verilerini mevcutsa dosyaya kaydedin
                if (certData != null && certData.Length > 0)
                {
                    File.WriteAllBytes("VbaCertificate.cer", certData);
                    Console.WriteLine("Certificate saved to file.");
                }
            }
            else
            {
                Console.WriteLine("VBA Project is not signed. CertRawData is not available.");
            }

            // Örnek senaryo: İmzalı VBA projesi olan bir çalışma kitabını yükleyin
            string signedWorkbookPath = "SignedWithVba.xlsm";
            if (File.Exists(signedWorkbookPath))
            {
                Workbook signedWorkbook = new Workbook(signedWorkbookPath);
                VbaProject signedVbaProject = signedWorkbook.VbaProject;

                if (signedVbaProject.IsSigned)
                {
                    byte[] signedCertData = signedVbaProject.CertRawData;
                    Console.WriteLine("Loaded workbook's VBA certificate data length: " + 
                        (signedCertData != null ? signedCertData.Length : 0));
                }
            }

            // Çalışma kitabını kaydedin
            workbook.Save("VbaProjectCertRawDataDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


