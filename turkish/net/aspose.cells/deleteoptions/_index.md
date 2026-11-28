---
title: "Sınıf DeleteOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DeleteOptions sınıfı. Satırların/ sütunların silinmesi ayarını temsil eder."
type: docs
url: /tr/net/aspose.cells/deleteoptions/
---
## DeleteOptions class

Satırları/sütunları silme ayarını temsil eder.

```csharp
public class DeleteOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [DeleteOptions](deleteoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [FormulaChangeMonitor](../../aspose.cells/deleteoptions/formulachangemonitor/) { get; set; } | Silme nedeniyle oluşan değişiklikleri izlemek için monitörü alır/ayarlar. |
| [UpdateReference](../../aspose.cells/deleteoptions/updatereference/) { get; set; } | Diğer çalışma sayfalarındaki başvuruların güncellenip güncellenmeyeceğini gösterir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DeleteOptionsDemo
    {
        public static void DeleteOptionsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");

            // Orijinal veriyi görüntüle
            Console.WriteLine("Original Data:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            // DeleteOptions oluştur
            DeleteOptions options = new DeleteOptions
            {
                UpdateReference = true // Set to true to update references in other worksheets
            };

            // İkinci satırı sil (Banana)
            sheet.Cells.DeleteRow(2, options.UpdateReference);

            // Silme işleminden sonra veriyi görüntüle
            Console.WriteLine("\nData After Deletion:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("DeleteOptionsExample.xlsx");
            workbook.Save("DeleteOptionsExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


