---
title: "ContentTypeProperty.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ContentTypeProperty özelliği. Nesnenin adını döndürür veya ayarlar"
type: docs
url: /tr/net/aspose.cells.properties/contenttypeproperty/name/
---
## ContentTypeProperty.Name property

Nesnenin adını döndürür veya ayarlar.

```csharp
public string Name { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Adı "ss" olan bir içerik türü özelliği ekle
            workbook.ContentTypeProperties.Add("ss", "bb", "text");
            
            // XLS formatında kaydet
            workbook.Save("example.xls");
            
            // Çalışma kitabını yeniden yükle ve Name özelliğini doğrula
            workbook = new Workbook("example.xls");
            Console.WriteLine("Name property in XLS: " + workbook.ContentTypeProperties[0].Name);
            
            // XLSX formatında kaydet
            workbook.Save("example.xlsx");
            
            // Yeniden yükle ve tekrar doğrula
            workbook = new Workbook("example.xlsx");
            Console.WriteLine("Name property in XLSX: " + workbook.ContentTypeProperties[0].Name);
        }
    }
}
```

### Ayrıca Bakınız

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


