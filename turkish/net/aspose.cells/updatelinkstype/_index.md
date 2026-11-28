---
title: "Enum UpdateLinksType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.UpdateLinksType enum. Çalışma kitabı açıldığında diğer çalışma kitaplarına olan bağlantıların nasıl güncelleneceğini temsil eder"
type: docs
url: /tr/net/aspose.cells/updatelinkstype/
---
## UpdateLinksType enumeration

Çalışma kitabı açıldığında diğer çalışma kitaplarına olan bağlantıların nasıl güncelleneceğini temsil eder.

```csharp
public enum UpdateLinksType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| UserSet | `0` | Kullanıcıyı güncellemeye yönlendir. |
| Never | `1` | Güncellenmesin ve kullanıcıya sorulmasın. |
| Always | `2` | Her zaman güncelle. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UpdateLinksTypeDemo
    {
        public static void UpdateLinksTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabı ayarlarına erişin
            WorkbookSettings settings = workbook.Settings;

            // UpdateLinksType'ı Her zaman güncelle olarak ayarlayın
            settings.UpdateLinksType = UpdateLinksType.Always;

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("External Link Example");
            worksheet.Cells["A2"].PutValue("Data");

            // Çalışma kitabını kaydedin
            workbook.Save("UpdateLinksTypeExample.xlsx");

            // Mevcut UpdateLinksType ayarını çıktı olarak ver
            Console.WriteLine("UpdateLinksType is set to: " + settings.UpdateLinksType);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


