---
title: "Sınıf DigitalSignature"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DigitalSignatures.DigitalSignature sınıfı. Dosyadaki imza"
type: docs
url: /tr/net/aspose.cells.digitalsignatures/digitalsignature/
---
## DigitalSignature class

Dosyada imza.

```csharp
public class DigitalSignature
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [DigitalSignature](digitalsignature/#constructor_1)(X509Certificate2, string, DateTime) | digitalSignature yapıcı. .Net uygulamasını kullanır. |
| [DigitalSignature](digitalsignature/#constructor)(byte[], string, string, DateTime) | digitalSignature yapıcı. Bouncy Castle uygulamasını kullanır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Certificate](../../aspose.cells.digitalsignatures/digitalsignature/certificate/) { get; set; } | Belgeyi imzalamak için kullanılan sertifika nesnesi. |
| [Comments](../../aspose.cells.digitalsignatures/digitalsignature/comments/) { get; set; } | İmzanın amacı. |
| [Id](../../aspose.cells.digitalsignatures/digitalsignature/id/) { get; set; } | Belge içeriğinde depolanan imza satırının GUID'iyle çapraz referans yapılabilen bir GUID belirtir. Varsayılan değer Boş (tüm sıfırlar) GUID'dir. |
| [Image](../../aspose.cells.digitalsignatures/digitalsignature/image/) { get; set; } | Dijital imza için bir görüntü belirtir. Varsayılan değer null'dur. |
| [IsValid](../../aspose.cells.digitalsignatures/digitalsignature/isvalid/) { get; } | Bu dijital imza geçerli ve belge değiştirilmemişse, bu değer doğru olacaktır. |
| [ProviderId](../../aspose.cells.digitalsignatures/digitalsignature/providerid/) { get; set; } | İmza sağlayıcısının sınıf kimliğini (class ID) belirtir. Varsayılan değer Boş (tüm sıfırlar) GUID'dir. |
| [SignTime](../../aspose.cells.digitalsignatures/digitalsignature/signtime/) { get; set; } | Belgenin imzalandığı zaman. |
| [Text](../../aspose.cells.digitalsignatures/digitalsignature/text/) { get; set; } | Dijital imzada gerçek imzanın metnini belirtir. Varsayılan değer Boş'tur. |
| [XAdESType](../../aspose.cells.digitalsignatures/digitalsignature/xadestype/) { get; set; } | XAdES türü. Varsayılan değer Yok (XAdES kapalı). |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Security.Cryptography.X509Certificates;

    public class DigitalSignaturesClassDigitalSignatureDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Digital Signature Demo");

            try
            {
                // Sertifika yapıcı kullanarak bir dijital imza oluşturun
                X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
                DigitalSignature signature = new DigitalSignature(
                    certificate,
                    "Document signed for approval",
                    DateTime.Now);

                // Ek özellikleri ayarla
                signature.Id = Guid.NewGuid();
                signature.Text = "Approved";
                signature.XAdESType = XAdESType.XAdES;

                // Çalışma kitabına imza ekle
                DigitalSignatureCollection signatures = new DigitalSignatureCollection();
                signatures.Add(signature);
                workbook.SetDigitalSignature(signatures);

                // İmza bilgilerini göster
                Console.WriteLine($"Signature added: {signature.Comments}");
                Console.WriteLine($"Sign time: {signature.SignTime}");
                Console.WriteLine($"Signature ID: {signature.Id}");

                // İmzalı çalışma kitabını kaydet
                workbook.Save("DigitalSignatureDemo.xlsx");
                Console.WriteLine("Workbook signed and saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DigitalSignature: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


