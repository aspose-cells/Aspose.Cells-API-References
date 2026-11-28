---
title: "Worksheet.AllowEditRanges"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Çalışma sayfasındaki düzenleme izin aralığı koleksiyonunu alır"
type: docs
url: /tr/net/aspose.cells/worksheet/alloweditranges/
---
## Worksheet.AllowEditRanges property

Çalışma sayfasındaki izin verilen düzenleme aralığı koleksiyonunu alır.

```csharp
public ProtectedRangeCollection AllowEditRanges { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyAllowEditRangesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir düzenleme izin aralığı ekle
            int index = worksheet.AllowEditRanges.Add("r1", 0, 0, 1, 1);
            ProtectedRange range = worksheet.AllowEditRanges[index];
            range.Password = "password123";

            // Çalışma sayfasını koru
            worksheet.Protect(ProtectionType.All);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");

            // Kaydedilmiş çalışma kitabını doğrulamak için yükle
            Workbook verifyWorkbook = new Workbook("output.xlsx");
            ProtectedRange verifyRange = verifyWorkbook.Worksheets[0].AllowEditRanges[0];
            Console.WriteLine("Is protected with password: " + verifyRange.IsProtectedWithPassword);
        }
    }
}
```

### Ayrıca Bakınız

* class [ProtectedRangeCollection](../../protectedrangecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


