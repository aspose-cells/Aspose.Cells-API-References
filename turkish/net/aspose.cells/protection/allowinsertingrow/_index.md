---
title: "Protection.AllowInsertingRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Protection özelliği. Korunan bir çalışma sayfasında satır eklemenin izin verilip verilmediğini temsil eder."
type: docs
url: /tr/net/aspose.cells/protection/allowinsertingrow/
---
## Protection.AllowInsertingRow property

Korunan bir çalışma sayfasında satır eklemenin izin verilip verilmediğini temsil eder

```csharp
public bool AllowInsertingRow { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Koruma ayarlarına erişin
            Protection protection = worksheet.Protection;

            // Koruma altında iken satır eklemeyi etkinleştir
            protection.AllowInsertingRow = true;
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            // Bir satır eklemeyi deneyin (AllowInsertingRow true olduğu için çalışmalıdır)
            worksheet.Cells.InsertRow(0);

            // Çalışma kitabını kaydedin
            workbook.Save("AllowInsertingRowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


