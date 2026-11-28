---
title: "Protection.AllowDeletingColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Protection özelliği. Korunan bir çalışma sayfasında sütunların silinmesine izin verilip verilmediğini temsil eder"
type: docs
url: /tr/net/aspose.cells/protection/allowdeletingcolumn/
---
## Protection.AllowDeletingColumn property

Korunan bir çalışma sayfasında sütunların silinmesinin izin verilip verilmediğini temsil eder.

```csharp
public bool AllowDeletingColumn { get; set; }
```

### Açıklamalar

Silinecek hücreleri içeren sütunlar, sayfa korunduğunda kilidi açılmış olmalı ve "Select unlocked cells" seçeneği etkinleştirilmiş olmalıdır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowDeletingColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfası korumasını etkinleştir
            Protection protection = worksheet.Protection;
            protection.AllowDeletingColumn = true;
            worksheet.Protect(ProtectionType.All);

            // Ayarı doğrula
            Console.WriteLine("AllowDeletingColumn: " + protection.AllowDeletingColumn);

            // Bir sütunu silmeyi deneyin (AllowDeletingColumn true olduğu için çalışmalıdır)
            worksheet.Cells.DeleteColumn(0);
            Console.WriteLine("Column deleted successfully");

            // Sütun silmeyi devre dışı bırakın
            protection.AllowDeletingColumn = false;

            // Başka bir sütunu silmeyi deneyin (başarısız olmalıdır)
            try
            {
                worksheet.Cells.DeleteColumn(1);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Failed to delete column: " + ex.Message);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


