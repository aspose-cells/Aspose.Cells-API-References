---
title: "BuiltInDocumentPropertyCollection.Lines"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BuiltInDocumentPropertyCollection özelliği. Belgede satır sayısının tahmini bir değerini temsil eder"
type: docs
url: /tr/net/aspose.cells.properties/builtindocumentpropertycollection/lines/
---
## BuiltInDocumentPropertyCollection.Lines property

Belgede satır sayısının tahmini bir değerini temsil eder.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Lines { get; set; }
```

### Açıklamalar

Aspose.Cells, belgeyi değiştirdiğinizde bu özelliği güncellemez.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyLinesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Yerleşik belge özelliklerine eriş
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Mevcut Lines değerini göster (belgedeki satır sayısının tahmini)
            Console.WriteLine("Current Lines value: " + properties.Lines);
            
            // Lines özelliği için yeni bir değer ayarlayın
            properties.Lines = 150;
            
            // Özelliğin amacını göstermek için bazı içerikler ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Line " + (i + 1);
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("PropertyLinesDemo.xlsx");
            
            // Not: Lines özelliği bir tahmindir ve gerçek içerikle otomatik olarak güncellenmez
            // Özellikle belge meta verileri amacıyla kullanılır
        }
    }
}
```

### Ayrıca Bakınız

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


