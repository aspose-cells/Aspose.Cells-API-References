---
title: "DigitalSignature.Comments"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DigitalSignature özelliği. İmzanın amacı"
type: docs
url: /tr/net/aspose.cells.digitalsignatures/digitalsignature/comments/
---
## DigitalSignature.Comments property

İmzanın amacı.

```csharp
public string Comments { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyCommentsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Örnek veri ekleyin
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Digital Signature with Comments");

            // Yorumlarla dijital imza oluşturun
            DigitalSignature signature = new DigitalSignature(
                File.ReadAllBytes("sample.pfx"), 
                "password", 
                "Sample Signature with Comments", 
                DateTime.Now)
            {
                Comments = "This is a test comment for the digital signature"
            };

            // İmzayı koleksiyona ekleyin
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Çalışma kitabını imzalayın
            workbook.SetDigitalSignature(dsCollection);

            // İmzalı çalışma kitabını kaydet
            string outputPath = "SignedWithComments.xlsx";
            workbook.Save(outputPath);

            // İmzayı doğrulayın ve bilgi gösterin
            Workbook signedWorkbook = new Workbook(outputPath);
            DigitalSignatureCollection signatures = signedWorkbook.GetDigitalSignature();

            foreach (DigitalSignature ds in signatures)
            {
                Console.WriteLine($"Comments: {ds.Comments}");
                Console.WriteLine($"Sign Time: {ds.SignTime}");
                Console.WriteLine($"Is Valid: {ds.IsValid}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


