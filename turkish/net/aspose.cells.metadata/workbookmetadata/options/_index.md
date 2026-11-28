---
title: "WorkbookMetadata.Options"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookMetadata özelliği. Meta verilerin seçeneklerini alır"
type: docs
url: /tr/net/aspose.cells.metadata/workbookmetadata/options/
---
## WorkbookMetadata.Options property

Meta verinin seçeneklerini alır.

```csharp
public MetadataOptions Options { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class WorkbookMetadataPropertyOptionsDemo
    {
        public static void Run()
        {
            // Belge özellikleri için meta veri seçenekleri oluştur
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            options.Password = "test123";
            options.KeyLength = 128;

            // Seçeneklerle yeni bir çalışma kitabı meta veri örneği oluştur
            WorkbookMetadata metadata = new WorkbookMetadata("sample.xlsx", options);

            // Mevcut seçenek değerlerini göster
            Console.WriteLine("Metadata Type: " + metadata.Options.MetadataType);
            Console.WriteLine("Password: " + metadata.Options.Password);
            Console.WriteLine("Key Length: " + metadata.Options.KeyLength);

            // Yerleşik belge özelliklerine eriş
            var builtInProps = metadata.BuiltInDocumentProperties;
            builtInProps.Author = "Aspose Developer";
            builtInProps.Title = "Metadata Demo";

            // Özel belge özellikleri ekle
            var customProps = metadata.CustomDocumentProperties;
            customProps.Add("Department", "Development");
            customProps.Add("Project", "Metadata API");

            // Meta veri değişikliklerini kaydet
            metadata.Save("output.xlsx");

            // Şifreleme için yeni seçenekler oluştur
            MetadataOptions newOptions = new MetadataOptions(MetadataType.Encryption);
            newOptions.Password = "newpassword";
            newOptions.KeyLength = 256;
            
            WorkbookMetadata encryptedMetadata = new WorkbookMetadata("sample.xlsx", newOptions);
            encryptedMetadata.Save("encrypted_output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


