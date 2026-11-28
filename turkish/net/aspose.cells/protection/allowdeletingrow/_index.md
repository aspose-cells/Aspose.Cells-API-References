---
title: "Protection.AllowDeletingRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Protection özelliği. Korunan bir çalışma sayfasında satır silmeye izin verilip verilmediğini gösterir"
type: docs
url: /tr/net/aspose.cells/protection/allowdeletingrow/
---
## Protection.AllowDeletingRow property

Korunan bir çalışma sayfasında satırların silinmesinin izin verilip verilmediğini temsil eder.

```csharp
public bool AllowDeletingRow { get; set; }
```

### Açıklamalar

Silinecek hücreleri içeren satırların, sayfa korunduğunda kilidi açılmış olması gerekir ve "Select unlocked cells" seçeneği etkinleştirilmelidir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowDeletingRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Koruma ayarlarını belirle
            Protection protection = sheet.Protection;
            protection.AllowDeletingRow = true;
            protection.AllowSorting = true;
            protection.AllowFiltering = true;
            protection.AllowFormattingColumn = true;

            // Çalışma sayfasını koru
            sheet.Protect(ProtectionType.All);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");

            // Ayarları doğrulamak için kaydedilmiş çalışma kitabını yükle
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];

            // AllowDeletingRow ve diğer özellikleri doğrulayın
            Console.WriteLine("AllowDeletingRow: " + loadedSheet.Protection.AllowDeletingRow);
            Console.WriteLine("AllowSorting: " + loadedSheet.Protection.AllowSorting);
            Console.WriteLine("AllowFiltering: " + loadedSheet.Protection.AllowFiltering);
            Console.WriteLine("AllowFormattingColumn: " + loadedSheet.Protection.AllowFormattingColumn);
        }
    }
}
```

### Ayrıca Bakınız

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


