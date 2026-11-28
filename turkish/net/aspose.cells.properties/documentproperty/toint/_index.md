---
title: "DocumentProperty.ToInt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DocumentProperty yöntemi. Özellik değerini tamsayı olarak döndürür"
type: docs
url: /tr/net/aspose.cells.properties/documentproperty/toint/
---
## DocumentProperty.ToInt method

Özellik değerini integer olarak döndürür.

```csharp
public int ToInt()
```

### Açıklamalar

Özellik tipi PropertyType.Number değilse bir istisna fırlatır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToIntDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Özel belge özellikleri koleksiyonunu al
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Sayısal bir özel özellik ekle
            customProperties.Add("Revision", 5);

            // Özelliği al ve ToInt() kullanarak int'e dönüştür
            DocumentProperty revisionProperty = customProperties["Revision"];
            int revisionValue = revisionProperty.ToInt();
            
            // Sonucu çıktı olarak ver
            Console.WriteLine($"Revision (as int): {revisionValue}");

            // Çalışma kitabını kaydedin
            workbook.Save("DocumentPropertyToIntExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


