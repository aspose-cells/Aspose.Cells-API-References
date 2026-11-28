---
title: "Protection.AllowInsertingColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Protection özelliği. Korunan bir çalışma sayfasında sütun eklemenin izin verilip verilmediğini temsil eder."
type: docs
url: /tr/net/aspose.cells/protection/allowinsertingcolumn/
---
## Protection.AllowInsertingColumn property

Korunan bir çalışma sayfasında sütun eklemenin izin verilip verilmediğini temsil eder

```csharp
public bool AllowInsertingColumn { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Koruma ayarlarını alın
            Protection protection = worksheet.Protection;

            // AllowInsertingColumn değerini true olarak ayarlayın
            protection.AllowInsertingColumn = true;

            // Ayarı doğrula
            Console.WriteLine("AllowInsertingColumn is set to: " + protection.AllowInsertingColumn);

            // Çalışma sayfasını şifreyle koruyun (Workbook.Protect yöntemi kullanılarak)
            workbook.Protect(ProtectionType.All, "password123");
            protection.AllowInsertingColumn = true; // Explicitly set again to demonstrate

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


