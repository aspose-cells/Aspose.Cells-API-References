---
title: "DigitalSignature.DigitalSignature"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DigitalSignature yapıcı. digitalSignature'ın yapıcısı. .Net uygulamasını kullanır"
type: docs
url: /tr/net/aspose.cells.digitalsignatures/digitalsignature/digitalsignature/
---
## DigitalSignature(X509Certificate2, string, DateTime) {#constructor_1}

digitalSignature yapıcı. .Net uygulamasını kullanır.

```csharp
public DigitalSignature(X509Certificate2 certificate, string comments, DateTime signTime)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sertifika | X509Certificate2 | Belgeyi imzalamak için kullanılan sertifika nesnesi. |
| yorumlar | String | İmzanın amacı. |
| signTime | DateTime | Belgenin imzalandığı utc zamanı. |

### Örnekler

```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignatureMethodCtorWithX509Certificate2StringDateTimeDemo
    {
        public static void Run()
        {
            // Bir dijital imza koleksiyonu oluşturun
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            
            // Özel anahtarlı sertifikayı yükle
            X509Certificate2 certificate = new X509Certificate2("mykey2.pfx", "123456");
            
            // Sertifika, amaç ve zaman damgası ile dijital imza oluştur
            DigitalSignature signature = new DigitalSignature(
                certificate, 
                "Document approval", 
                DateTime.Now);
                
            signatures.Add(signature);
            
            // Yeni bir çalışma kitabı oluştur ve imzala
            Workbook workbook = new Workbook();
            workbook.SetDigitalSignature(signatures);
            workbook.Save("signed_document.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)

---

## DigitalSignature(byte[], string, string, DateTime) {#constructor}

digitalSignature yapıcı. Bouncy Castle uygulamasını kullanır.

```csharp
public DigitalSignature(byte[] rawData, string password, string comments, DateTime signTime)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rawData | Byte[] | X.509 sertifikasından veri içeren bir bayt dizisi. |
| parola | String | X.509 sertifika verilerine erişmek için gereken şifre. |
| yorumlar | String | İmzanın amacı. |
| signTime | DateTime | Belgenin imzalandığı utc zamanı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.IO;

    public class DigitalSignatureConstructorWithByteArrayStringStringDateTimeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Biraz örnek içerik ekle
            worksheet.Cells["A1"].PutValue("Digitally Signed Document");
            
            try
            {
                // Sertifika dosyasını bayt dizisi olarak yükle (gerçek sertifika yolu ile değiştir)
                string certPath = "certificate.pfx";
                byte[] certData = File.ReadAllBytes(certPath);
                
                // Dijital imza parametrelerini oluştur
                string password = "certificate_password";
                string comments = "Approved by John Doe";
                DateTime signTime = DateTime.Now;
                
                // Yapıcıyı (Byte[], String, String, DateTime) ile çağır
                DigitalSignature signature = new DigitalSignature(certData, password, comments, signTime);
                
                // Bir DigitalSignatureCollection oluştur ve imzayı ona ekle
                DigitalSignatureCollection signatures = new DigitalSignatureCollection();
                signatures.Add(signature);
                
                // İmzaları çalışma kitabına ekle
                workbook.AddDigitalSignature(signatures);
                
                Console.WriteLine("Digital signature added successfully with parameters (Byte[], String, String, DateTime)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing constructor method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("DigitalSignatureDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


