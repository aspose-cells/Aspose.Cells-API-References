---
title: "DocumentProperty.ToDouble"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DocumentProperty yöntemi. Özellik değerini double olarak döndürür"
type: docs
url: /tr/net/aspose.cells.properties/documentproperty/todouble/
---
## DocumentProperty.ToDouble method

Özellik değerini double olarak döndürür.

```csharp
public double ToDouble()
```

### Açıklamalar

Özellik türü PropertyType.Float değilse bir istisna fırlatır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToDoubleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Özel belge özellikleri koleksiyonunu al
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Sayısal bir özellik ekleyin
            customProperties.Add("Rating", 4.75);

            // Özelliği alın ve double'a dönüştürün
            DocumentProperty ratingProperty = customProperties["Rating"];
            double ratingValue = ratingProperty.ToDouble();

            // Sonucu çıktı olarak ver
            Console.WriteLine($"Rating: {ratingValue}");

            // Çalışma kitabını kaydedin
            workbook.Save("DocumentPropertyToDoubleExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


