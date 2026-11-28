---
title: "Worksheet.Protection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Bir çalışma sayfası için mevcut olan çeşitli koruma seçeneklerini temsil eder. ExcelXP ve sonraki sürümlerde gelişmiş koruma seçeneklerini destekler"
type: docs
url: /tr/net/aspose.cells/worksheet/protection/
---
## Worksheet.Protection property

Bir çalışma sayfası için mevcut olan çeşitli koruma seçeneklerini temsil eder. ExcelXP ve sonraki sürümlerde gelişmiş koruma seçeneklerini destekler.

```csharp
public Protection Protection { get; }
```

### Açıklamalar

Bu özellik, Excel dosyasının tüm sürümlerinde çalışma sayfasını koruyabilir ve ExcelXP ve sonraki sürümlerde gelişmiş koruma seçeneklerini destekler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyProtectionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Koruma özelliklerine eriş
            Protection protection = sheet.Protection;
            
            // Koruma özelliklerini ayarla
            protection.AllowEditingObject = false;
            protection.AllowEditingScenario = false;
            
            // Çalışma sayfasını koru (IsProtectedWithPassword'ı doğrudan ayarlamak yerine Protect yöntemini kullanarak)
            sheet.Protect(ProtectionType.All, "password123", null);

            // Çalışma kitabını kaydedin
            workbook.Save("WorksheetProtectionDemo.xlsx");

            // Koruma ayarlarını doğrula
            Console.WriteLine("AllowEditingObject: " + protection.AllowEditingObject);
            Console.WriteLine("AllowEditingScenario: " + protection.AllowEditingScenario);
        }
    }
}
```

### Ayrıca Bakınız

* class [Protection](../../protection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


