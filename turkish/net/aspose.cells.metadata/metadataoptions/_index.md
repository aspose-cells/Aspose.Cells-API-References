---
title: "Sınıf MetadataOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Metadata.MetadataOptions sınıfı. Dosyanın meta verisini yükleme seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells.metadata/metadataoptions/
---
## MetadataOptions class

Dosyanın meta verilerini yükleme seçeneklerini temsil eder.

```csharp
public class MetadataOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [MetadataOptions](metadataoptions/)(MetadataType) | Meta veriyi yükleme seçeneklerini oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [KeyLength](../../aspose.cells.metadata/metadataoptions/keylength/) { get; set; } | Anahtar uzunluğu. |
| [MetadataType](../../aspose.cells.metadata/metadataoptions/metadatatype/) { get; } | Yüklenen meta verinin türünü alır ve ayarlar. |
| [Password](../../aspose.cells.metadata/metadataoptions/password/) { get; set; } | Workbook dosya şifreleme parolasını temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class MetadataOptionsDemo
    {
        public static void MetadataOptionsExample()
        {
            // Belirli bir MetadataType ile MetadataOptions örneği oluştur
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Özellikleri ayarla
            options.Password = "your_password";
            options.KeyLength = 256;

            // Mevcut bir çalışma kitabından meta veriyi yükle
            WorkbookMetadata metadata = new WorkbookMetadata("MetadataOptionsExample_original.xlsx", options);

            // Özel bir belge özelliği ekle
            metadata.CustomDocumentProperties.Add("Author", "John Doe");

            // Meta veri değişikliklerini yeni bir dosyaya kaydet
            metadata.Save("MetadataOptionsExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


