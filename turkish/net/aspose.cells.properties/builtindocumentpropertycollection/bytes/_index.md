---
title: "BuiltInDocumentPropertyCollection.Bytes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BuiltInDocumentPropertyCollection özelliği. Belgedeki bayt sayısının tahmini bir değerini temsil eder"
type: docs
url: /tr/net/aspose.cells.properties/builtindocumentpropertycollection/bytes/
---
## BuiltInDocumentPropertyCollection.Bytes property

Belgedeki bayt sayısının tahmini bir değerini temsil eder.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Bytes { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyBytesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Yerleşik belge özelliklerine eriş
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Mevcut Bytes değerini göster (belge boyutunun tahmini)
            Console.WriteLine("Current Bytes value: " + properties.Bytes);

            // Boyutu etkileyecek şekilde bazı içerikler ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data to increase document size");
            for (int i = 2; i <= 100; i++)
            {
                worksheet.Cells["A" + i].PutValue("Line " + i);
            }

            // Bytes özelliğini manuel olarak güncelleyin (normalde otomatik olarak hesaplanır).
            properties.Bytes = 5000;
            Console.WriteLine("Updated Bytes value: " + properties.Bytes);

            // Kaydedilmiş dosyada özelliği görmek için çalışma kitabını kaydedin
            workbook.Save("PropertyBytesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


