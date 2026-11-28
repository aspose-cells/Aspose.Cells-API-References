---
title: "Enum MetadataType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Metadata.MetadataType enum. Metaverinin türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.metadata/metadatatype/
---
## MetadataType enumeration

Meta verinin türünü temsil eder.

```csharp
[Flags]
public enum MetadataType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Encryption | `1` | Dosyayı şifreler. |
| Decryption | `2` | Dosyanın şifresini çözer. |
| DocumentProperties | `4` | Dosyanın özelliklerini yükle. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Metadata;
    using Aspose.Cells.Properties;
    using System;
    using System.IO;

    public class MetadataTypeDemo
    {
        public static void MetadataTypeExample()
        {
            // Dosya yolunu tanımla
            string filePath = "MetadataTypeExample_original.xlsx";

            // DocumentProperties için MetadataOptions oluştur
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Çalışma kitabı meta verilerini yükle
            WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);

            // Yerleşik belge özelliklerine eriş
            BuiltInDocumentPropertyCollection builtInProperties = metadata.BuiltInDocumentProperties;

            // Özel belge özelliklerine eriş
            CustomDocumentPropertyCollection customProperties = metadata.CustomDocumentProperties;

            // Bazı yerleşik özellikleri göster
            Console.WriteLine("Title: " + builtInProperties["Title"]);
            Console.WriteLine("Author: " + builtInProperties["Author"]);
            Console.WriteLine("Company: " + builtInProperties["Company"]);

            // Özel bir özellik ekle
            customProperties.Add("MyCustomProperty", "CustomValue");

            // farklı bir dosyaya kaydet
            string newFilePath = "MetadataTypeExample.xlsx";
            metadata.Save(newFilePath);

            Console.WriteLine("Metadata updated and saved successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


