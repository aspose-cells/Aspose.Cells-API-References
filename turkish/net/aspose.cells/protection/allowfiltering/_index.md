---
title: "Protection.AllowFiltering"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Protection özelliği. Kullanıcının sayfa korunmadan önce oluşturulan bir AutoFilter'ı kullanmasına izin verilip verilmediğini temsil eder"
type: docs
url: /tr/net/aspose.cells/protection/allowfiltering/
---
## Protection.AllowFiltering property

Korunan bir çalışma sayfası korunmadan önce oluşturulan bir Otomatik Filtreyi kullanma izni olup olmadığını temsil eder.

```csharp
public bool AllowFiltering { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFilteringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfası korumasını etkinleştir
            worksheet.Protect(ProtectionType.All);
            
            // AllowFiltering özelliğini true olarak ayarlayın
            worksheet.Protection.AllowFiltering = true;
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // Özelliğin doğru kaydedildiğini doğrulayın
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("AllowFiltering: " + 
                loadedWorkbook.Worksheets[0].Protection.AllowFiltering);
        }
    }
}
```

### Ayrıca Bakınız

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


