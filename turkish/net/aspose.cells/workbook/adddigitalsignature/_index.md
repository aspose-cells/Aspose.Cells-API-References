---
title: "Workbook.AddDigitalSignature"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. OOXML elektronik tablo dosyasına (Excel2007 ve sonrası) dijital imza ekler"
type: docs
url: /tr/net/aspose.cells/workbook/adddigitalsignature/
---
## Workbook.AddDigitalSignature method

OOXML elektronik tablo dosyasına (Excel2007 ve sonrası) dijital imza ekler.

```csharp
public void AddDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### Açıklamalar

Yalnızca OOXML elektronik tablo dosyasına Xmldsig Dijital İmza eklemeyi destekler

### Örnekler

```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class WorkbookMethodAddDigitalSignatureWithDigitalSignatureCollectionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Örnek veri ekleyin
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Digital Signature");

            // Sertifikayı yükle (kendi sertifika yolunuz ve şifrenizle değiştirin)
            X509Certificate2 certificate = new X509Certificate2("DrWatson.pfx", "1234567890");

            // Dijital imza oluşturun
            DigitalSignature digitalSignature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);

            // Dijital imza koleksiyonu oluşturun ve imza ekleyin
            DigitalSignatureCollection digitalSignatureCollection = new DigitalSignatureCollection();
            digitalSignatureCollection.Add(digitalSignature);

            // Çalışma kitabına dijital imza ekleyin
            workbook.AddDigitalSignature(digitalSignatureCollection);

            // Çalışma kitabını kaydedin
            workbook.Save("DigitallySignedWorkbook.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


