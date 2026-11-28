---
title: "Protection.AllowFormattingRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Protection özelliği. Korunan bir çalışma sayfasında satır biçimlendirmeye izin verilip verilmediğini temsil eder."
type: docs
url: /tr/net/aspose.cells/protection/allowformattingrow/
---
## Protection.AllowFormattingRow property

Korunan bir çalışma sayfasında satır biçimlendirmesinin izin verilip verilmediğini temsil eder

```csharp
public bool AllowFormattingRow { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFormattingRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfası korumasını etkinleştir
            worksheet.Protect(ProtectionType.All);

            // Koruma ayarlarına eriş
            Protection protection = worksheet.Protection;

            // Diğer korumaları korurken satır biçimlendirmeye izin ver
            protection.AllowFormattingRow = true;

            // Çalışma kitabını kaydedin
            workbook.Save("Protection_AllowFormattingRow.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


