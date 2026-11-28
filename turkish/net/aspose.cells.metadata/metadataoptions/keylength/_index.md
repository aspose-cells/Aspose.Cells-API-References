---
title: "MetadataOptions.KeyLength"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MetadataOptions özelliği. Anahtar uzunluğu"
type: docs
url: /tr/net/aspose.cells.metadata/metadataoptions/keylength/
---
## MetadataOptions.KeyLength property

Anahtar uzunluğu.

```csharp
public int KeyLength { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class MetadataOptionsPropertyKeyLengthDemo
    {
        public static void Run()
        {
            // Belge özellikleri türüyle meta veri seçenekleri oluştur
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            
            // KeyLength dahil şifreleme özelliklerini ayarla
            options.Password = "secure_password";
            options.KeyLength = 256; // Using 256-bit encryption
            
            // Yeni bir çalışma kitabı için meta veri oluştur
            WorkbookMetadata metadata = new WorkbookMetadata("sample.xlsx", options);
            
            // Özel özellik ekle
            metadata.CustomDocumentProperties.Add("CreatedBy", "MetadataDemo");
            
            // Şifreleme ile kaydet
            metadata.Save("encrypted_sample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


