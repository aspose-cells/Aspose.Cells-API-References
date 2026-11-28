---
title: "WorkbookMetadata.CustomDocumentProperties"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookMetadata özelliği. Elektronik tablo için tüm özel belge özelliklerini temsil eden bir DocumentProperty koleksiyonu döndürür"
type: docs
url: /tr/net/aspose.cells.metadata/workbookmetadata/customdocumentproperties/
---
## WorkbookMetadata.CustomDocumentProperties property

Elektronik tabloyun tüm özel belge özelliklerini temsil eden bir [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) koleksiyonu döndürür.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class WorkbookMetadataPropertyCustomDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Kaynak ve hedef yollar
            string sourcePath = "example.xlsx";
            string destPath = "output.xlsx";

            // Belge özellikleri için meta veri seçenekleri oluştur
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            
            // Çalışma kitabı meta verisini başlat
            WorkbookMetadata meta = new WorkbookMetadata(sourcePath, options);
            
            // Özel belge özelliği ekle
            meta.CustomDocumentProperties.Add("Author", "John Doe");
            
            // Çalışma kitabını meta verilerle kaydet
            meta.Save(destPath);
            
            // Özel özelliği doğrula
            Workbook workbook = new Workbook(destPath);
            Console.WriteLine("Custom Property Value: " + 
                workbook.CustomDocumentProperties["Author"].Value);
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


