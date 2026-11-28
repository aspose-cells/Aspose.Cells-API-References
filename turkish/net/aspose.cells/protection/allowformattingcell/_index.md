---
title: "Protection.AllowFormattingCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Protection özelliği. Korumalı bir çalışma sayfasında hücre biçimlendirmesine izin verilip verilmediğini temsil eder."
type: docs
url: /tr/net/aspose.cells/protection/allowformattingcell/
---
## Protection.AllowFormattingCell property

Korunan bir çalışma sayfasında hücre biçimlendirmesinin izin verilip verilmediğini temsil eder.

```csharp
public bool AllowFormattingCell { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFormattingCellDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfası korumasını etkinleştir
            Protection protection = worksheet.Protection;
            
            // Bir işaretçi kullanarak çeşitli koruma özelliklerini ayarlayın.
            int flag = 0x40; // Only AllowFormattingCell flag is set
            protection.AllowFormattingCell = (flag & 0x40) != 0;

            // Ayarı doğrula
            Console.WriteLine("AllowFormattingCell is set to: " + protection.AllowFormattingCell);

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


