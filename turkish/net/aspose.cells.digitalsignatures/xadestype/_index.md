---
title: "XAdESType enum'ı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DigitalSignatures.XAdESType enum. XML Gelişmiş Elektronik İmza (XAdES) türü"
type: docs
url: /tr/net/aspose.cells.digitalsignatures/xadestype/
---
## XAdESType enumeration

XML Gelişmiş Elektronik İmza (XAdES) türü.

```csharp
public enum XAdESType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | XAdES kapalı. |
| XAdES | `1` | Temel XAdES. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.IO;
    using System.Security.Cryptography.X509Certificates;

    public class XAdESTypeDemo
    {
        public static void XAdESTypeExample()
        {
            // Kaynak dizin
            string sourceDir = "path_to_source_directory";
            // Çıktı dizini
            string outputDir = "path_to_output_directory";
            // Çalışma kitabını yükle
            Workbook workbook = new Workbook(Path.Combine(sourceDir, "XAdESTypeExample_original.xlsx"));

            // PFX dosyası için şifreyi tanımlayın
            string password = "pfxPassword";
            // PFX dosyasının yolu
            string pfxPath = Path.Combine(sourceDir, "pfxFile.pfx");

            // Dijital imza oluşturun
            DigitalSignature signature = new DigitalSignature(File.ReadAllBytes(pfxPath), password, "testXAdES", DateTime.Now);
            // XAdES türünü ayarlayın
            signature.XAdESType = XAdESType.XAdES;

            // Dijital imzaların bir koleksiyonunu oluşturun
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Dijital imzayı çalışma kitabına ayarlayın
            workbook.SetDigitalSignature(dsCollection);

            // Çalışma kitabını dijital imza ile kaydedin
            workbook.Save(Path.Combine(outputDir, "XAdESSignatureSupport_out.xlsx"));

            // Dijital imzayı doğrulayın
            Workbook signedWorkbook = new Workbook(Path.Combine(outputDir, "XAdESSignatureSupport_out.xlsx"));
            DigitalSignatureCollection signatures = signedWorkbook.GetDigitalSignature();

            foreach (DigitalSignature ds in signatures)
            {
                Console.WriteLine($"Comments: {ds.Comments}");
                Console.WriteLine($"Sign Time: {ds.SignTime}");
                Console.WriteLine($"Is Valid: {ds.IsValid}");
                Console.WriteLine($"XAdES Type: {ds.XAdESType}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


