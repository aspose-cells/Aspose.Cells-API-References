---
title: "Workbook.SetDigitalSignature"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Excel2007 ve sonraki sürümlerdeki bir elektronik tablo dosyasına dijital imza ekler"
type: docs
url: /tr/net/aspose.cells/workbook/setdigitalsignature/
---
## Workbook.SetDigitalSignature method

Bir elektronik tablo dosyasına (Excel2007 ve sonrası) dijital imza ekler.

```csharp
public void SetDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### Açıklamalar

Yalnızca Xmldsig Dijital İmza eklemeyi destekler

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetDigitalSignatureWithDigitalSignatureCollectionDemo
    {
        public static void Run()
        {
            // Kaynak dizin yolu
            string sourceDir = "SourceDirectory/";
            
            // Çıktı dizin yolu
            string outputDir = "OutputDirectory/";

            // Çalışma kitabını yükle
            Workbook workbook = new Workbook(sourceDir + "TestCert.xlsx");

            // Dijital imza koleksiyonu oluşturun
            DigitalSignatureCollection digitalSignatures = new DigitalSignatureCollection();

            // Sertifika dosyasını yükleyin
            string certPath = sourceDir + "certs\\sample.pfx";
            byte[] certData = File.ReadAllBytes(certPath);

            // Dijital imza oluşturun
            DigitalSignature signature = new DigitalSignature(certData, "1234567890", "Sample Signer", DateTime.Now);

            // İmzayı koleksiyona ekleyin
            digitalSignatures.Add(signature);

            // Çalışma kitabına dijital imza ayarlayın
            workbook.SetDigitalSignature(digitalSignatures);

            // Çalışma kitabını kaydedin
            workbook.Save(outputDir + "DigitallySignedWorkbook.xlsx");

            Console.WriteLine("Digital signature set successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


