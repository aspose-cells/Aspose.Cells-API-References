---
title: "DocumentProperty.ToDateTime"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DocumentProperty yöntemi. Özellik değerini yerel saat diliminde DateTime olarak döndürür"
type: docs
url: /tr/net/aspose.cells.properties/documentproperty/todatetime/
---
## DocumentProperty.ToDateTime method

Özellik değerini yerel saat diliminde DateTime olarak döndürür.

```csharp
public DateTime ToDateTime()
```

### Açıklamalar

Özellik tipi PropertyType.Date değilse bir istisna fırlatır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToDateTimeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Özel belge özellikleri koleksiyonunu al
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Bir datetime özelliği ekle
            DateTime currentTime = DateTime.Now;
            customProperties.Add("LastModified", currentTime);

            // Özelliği al ve DateTime'a dönüştür
            DocumentProperty lastModifiedProperty = customProperties["LastModified"];
            DateTime retrievedTime = lastModifiedProperty.ToDateTime();

            // Sonucu çıktı olarak ver
            Console.WriteLine($"Stored DateTime: {currentTime}");
            Console.WriteLine($"Retrieved DateTime: {retrievedTime}");

            // Çalışma kitabını kaydedin
            workbook.Save("DocumentPropertyDateTimeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


