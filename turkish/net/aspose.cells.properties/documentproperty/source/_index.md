---
title: "DocumentProperty.Source"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DocumentProperty özelliği. Bağlantılı içerik kaynağı"
type: docs
url: /tr/net/aspose.cells.properties/documentproperty/source/
---
## DocumentProperty.Source property

Bağlantılı içerik kaynağı.

```csharp
public string Source { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertySourceDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Özel belge özelliklerine eriş
            var properties = workbook.Worksheets.CustomDocumentProperties;

            // Özellikler ekleyin
            properties.Add("Author", "John Doe");
            properties.Add("CreatedDate", DateTime.Now);
            properties.Add("Revision", 1);
            
            // Özellikleri alın ve kaynaklarını gösterin
            Console.WriteLine("Property Sources:");
            Console.WriteLine($"Author: {properties["Author"].Source}");
            Console.WriteLine($"CreatedDate: {properties["CreatedDate"].Source}");
            Console.WriteLine($"Revision: {properties["Revision"].Source}");

            // Çalışma kitabını kaydedin
            workbook.Save("DocumentPropertiesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


