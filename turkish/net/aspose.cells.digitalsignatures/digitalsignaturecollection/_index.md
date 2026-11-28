---
title: "Class DigitalSignatureCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DigitalSignatures.DigitalSignatureCollection sınıfı. Bir belgeye eklenmiş dijital imzaların bir koleksiyonunu sağlar"
type: docs
url: /tr/net/aspose.cells.digitalsignatures/digitalsignaturecollection/
---
## DigitalSignatureCollection class

Bir belgeye eklenmiş dijital imzaların bir koleksiyonunu sağlar.

```csharp
public class DigitalSignatureCollection : IEnumerable
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [DigitalSignatureCollection](digitalsignaturecollection/)() | DigitalSignatureCollection sınıfının yapıcısı. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells.digitalsignatures/digitalsignaturecollection/add/)(DigitalSignature) | DigitalSignatureCollection'a bir imza ekleyin. |
| [GetEnumerator](../../aspose.cells.digitalsignatures/digitalsignaturecollection/getenumerator/)() | DigitalSignatureCollection için enumeratörü alın, bu enumeratör koleksiyon üzerinde yineleme yapmayı sağlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Security.Cryptography.X509Certificates;

    public class DigitalSignatureCollectionDemo
    {
        public static void DigitalSignatureCollectionExample()
        {
            // İmzalı bir kaynak dosyadan çalışma kitabını yükleyin.
            Workbook signedWorkbook = new Workbook(@"DigitalSignatureCollection_original.xlsx");

            // Çalışma kitabının dijital olarak imzalı olup olmadığını kontrol et
            Console.WriteLine("Is the workbook digitally signed? " + signedWorkbook.IsDigitallySigned);

            // Çalışma kitabından dijital imza koleksiyonunu alın.
            DigitalSignatureCollection existingDsc = signedWorkbook.GetDigitalSignature();

            if (existingDsc != null)
            {
                // Koleksiyondaki dijital imzalar üzerinde yineleme yapın.
                foreach (DigitalSignature existingDs in existingDsc)
                {
                    Console.WriteLine("Comments: " + existingDs.Comments);
                    Console.WriteLine("Sign Time: " + existingDs.SignTime);
                    Console.WriteLine("Is Valid: " + existingDs.IsValid);
                }

                // Yeni bir dijital imza oluşturun.
                X509Certificate2 certificate = new X509Certificate2("path_to_certificate.pfx", "password");
                DigitalSignature newSignature = new DigitalSignature(certificate, "New signature comment", DateTime.Now);

                // Yeni dijital imzayı koleksiyona ekleyin.
                existingDsc.Add(newSignature);
            }     
            

            // Çalışma kitabını yeni dijital imza ile kaydedin.
            signedWorkbook.Save("DigitalSignatureCollectionExample.xlsx");
            signedWorkbook.Save("DigitalSignatureCollectionExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


