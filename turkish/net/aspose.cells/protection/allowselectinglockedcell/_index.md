---
title: "Protection.AllowSelectingLockedCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Protection özelliği. Kullanıcının korumalı bir çalışma sayfasında kilitli hücreleri seçip seçemeyeceğini temsil eder."
type: docs
url: /tr/net/aspose.cells/protection/allowselectinglockedcell/
---
## Protection.AllowSelectingLockedCell property

Korunan bir çalışma sayfasında kilitli hücreleri seçme izni olup olmadığını temsil eder.

```csharp
public bool AllowSelectingLockedCell { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSelectingLockedCellDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Koruma ayarlarını belirle
            Protection protection = worksheet.Protection;
            
            // AllowSelectingLockedCell özelliğini göster
            protection.AllowSelectingLockedCell = true;
            Console.WriteLine("AllowSelectingLockedCell is set to: " + protection.AllowSelectingLockedCell);

            // Özelliği değiştir ve değişikliği göster
            protection.AllowSelectingLockedCell = false;
            Console.WriteLine("AllowSelectingLockedCell is now set to: " + protection.AllowSelectingLockedCell);

            // Çalışma sayfasını şifreyle koru
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            // Çalışma kitabını kaydedin
            workbook.Save("ProtectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


