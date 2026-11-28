---
title: "DocumentProperty.IsGeneratedName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DocumentProperty özelliği. Bu özellik OLE2 depolamasında bir adı yoksa ve yalnızca genel API için benzersiz bir ad oluşturulmuşsa true döndürür"
type: docs
url: /tr/net/aspose.cells.properties/documentproperty/isgeneratedname/
---
## DocumentProperty.IsGeneratedName property

Bu özelliğin OLE2 depolamasında bir adı yoksa ve yalnızca genel API için benzersiz bir ad oluşturulduysa true döndürür.

```csharp
public bool IsGeneratedName { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyPropertyIsGeneratedNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Yerleşik belge özelliklerine eriş
            DocumentPropertyCollection properties = workbook.Worksheets.BuiltInDocumentProperties;
            
            // Eklemek için özel belge özelliklerine eriş
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Özel bir özellik ekle
            DocumentProperty customProperty = customProperties.Add("CustomProperty", "Test Value");
            
            // Yerleşik özellik için IsGeneratedName'i göster
            DocumentProperty authorProperty = properties["Author"];
            Console.WriteLine("Author property IsGeneratedName: " + authorProperty.IsGeneratedName);
            
            // Özel özellik için IsGeneratedName'i göster
            Console.WriteLine("Custom property IsGeneratedName: " + customProperty.IsGeneratedName);

            // Bir özelliğin oluşturulmuş bir adı olabileceği bir senaryo oluştur
            // (Not: Pratikte, IsGeneratedName yalnızca okunur ve Aspose.Cells tarafından dahili olarak ayarlanır)
            DocumentProperty generatedNameProperty = properties["_PID_GUID"];
            if (generatedNameProperty != null)
            {
                Console.WriteLine("Generated name property IsGeneratedName: " + generatedNameProperty.IsGeneratedName);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("PropertyIsGeneratedNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


