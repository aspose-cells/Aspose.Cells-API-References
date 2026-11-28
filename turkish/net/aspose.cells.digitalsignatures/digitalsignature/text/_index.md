---
title: "DigitalSignature.Text"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DigitalSignature özelliği. Dijital imzada gerçek imzanın metnini belirtir. Varsayılan değer Boş"
type: docs
url: /tr/net/aspose.cells.digitalsignatures/digitalsignature/text/
---
## DigitalSignature.Text property

Dijital imzada gerçek imzanın metnini belirtir. Varsayılan değer Boş'tur.

```csharp
public string Text { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Security.Cryptography.X509Certificates;

    public class DigitalSignaturePropertyTextDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir test sertifikası oluşturun (gerçek senaryoda, geçerli bir sertifika kullanın)
            X509Certificate2 certificate = null;
            try
            {
                certificate = new X509Certificate2();
            }
            catch
            {
                Console.WriteLine("Could not create certificate. Using null for demonstration.");
            }

            // Bir dijital imza örneği oluşturun
            DigitalSignature signature = new DigitalSignature(
                certificate,
                "Sample signature comments",
                DateTime.Now);

            // Mevcut Text değerini göster (varsayılan boş)
            Console.WriteLine("Current Text value: " + signature.Text);

            // Text özelliği için yeni bir değer ayarlayın
            signature.Text = "Approved by John Doe";

            // Bir dijital imza koleksiyonu oluşturun ve imzayı ona ekleyin
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            signatures.Add(signature);

            // Dijital imzaları çalışma kitabına ekleyin
            workbook.AddDigitalSignature(signatures);

            // Çalışma kitabını dijital imza ile kaydedin
            try
            {
                workbook.Save("DigitalSignatureWithText.xlsx");
                Console.WriteLine("Workbook saved with digital signature text: " + signature.Text);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error saving workbook: " + ex.Message);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


