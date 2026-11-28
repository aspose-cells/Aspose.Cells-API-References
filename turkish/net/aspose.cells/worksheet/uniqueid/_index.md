---
title: "Worksheet.UniqueId"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Benzersiz kimliği alır ve ayarlar, 15DB5C3CA5A148AF8F253D86AC232D4F ile aynı"
type: docs
url: /tr/net/aspose.cells/worksheet/uniqueid/
---
## Worksheet.UniqueId property

Benzersiz kimliği alır ve ayarlar, {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F} ile aynı.

```csharp
public string UniqueId { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyUniqueIdDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma sayfası için benzersiz bir kimlik oluşturun
            string uniqueId = "{" + Guid.NewGuid().ToString() + "}";
            
            // İlk çalışma sayfasının UniqueId özelliğini ayarlayın
            workbook.Worksheets[0].UniqueId = uniqueId;
            
            // Çalışma kitabını kaydedin
            string outputPath = "SheetUniqueIdDemo.xlsx";
            workbook.Save(outputPath);
            
            // Çalışma kitabını yeniden yükleyerek UniqueId'nin kalıcı olduğunu doğrulayın
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // İşlevselliği göstermek için UniqueId'yi çıktılayın
            Console.WriteLine("Worksheet UniqueId: " + loadedWorkbook.Worksheets[0].UniqueId);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


