---
title: "MetadataOptions.Password"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MetadataOptions özelliği. Çalışma kitabı dosyası şifreleme parolasını temsil eder"
type: docs
url: /tr/net/aspose.cells.metadata/metadataoptions/password/
---
## MetadataOptions.Password property

Workbook dosya şifreleme parolasını temsil eder.

```csharp
public string Password { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class MetadataOptionsPropertyPasswordDemo
    {
        public static void Run()
        {
            // Parola korumalı meta veri seçenekleri oluştur
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            options.Password = "secure_password123";
            
            // Yeni bir çalışma kitabı oluştur ve önce kaydet
            Workbook workbook = new Workbook();
            string filePath = "ProtectedMetadata.xlsx";
            workbook.Save(filePath);
            
            // Kaydedilen dosyadan meta veriyi yükle
            WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);
            
            // Özel belge özelliği ekle
            metadata.CustomDocumentProperties.Add("CreatedBy", "MetadataDemo");
            
            // Meta veri ile kaydet
            metadata.Save(filePath);
        }
    }
}
```

### Ayrıca Bakınız

* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


