---
title: "DigitalSignature.IsValid"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DigitalSignature özelliği. Bu dijital imza geçerli ve belge değiştirilmemişse bu değer doğru (true) olacaktır."
type: docs
url: /tr/net/aspose.cells.digitalsignatures/digitalsignature/isvalid/
---
## DigitalSignature.IsValid property

Bu dijital imza geçerli ve belge değiştirilmemişse, bu değer doğru olacaktır.

```csharp
public bool IsValid { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;
using System.IO;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyIsValidDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma sayfasına bazı veriler ekle
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Digital Signature");
            
            // Önce çalışma kitabını kaydedin
            string outputPath = "signed_example.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);

            // Bir dijital imza koleksiyonu oluşturun
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            
            // Bir dijital imza oluşturun (gerçek senaryoda, uygun sertifika kullanın)
            // İlk parametre, sertifika verisinin byte[] olması gerekir
            byte[] certificateData = File.ReadAllBytes("test.pfx");
            DigitalSignature signature = new DigitalSignature(
                certificateData, 
                "test123", 
                "Test Signature", 
                DateTime.Now);
                
            signatures.Add(signature);
            
            // Çalışma kitabını imzalayın
            workbook.SetDigitalSignature(signatures);
            workbook.Save(outputPath, SaveFormat.Xlsx);

            // İmzayı doğrulayın
            Workbook signedWorkbook = new Workbook(outputPath);
            DigitalSignatureCollection loadedSignatures = signedWorkbook.GetDigitalSignature();
            
            foreach (DigitalSignature sig in loadedSignatures)
            {
                Console.WriteLine("Signature is valid: " + sig.IsValid);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


