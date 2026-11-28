---
title: "HtmlHiddenColDisplayType enum'ı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.HtmlHiddenColDisplayType enum'ı. HTML'de gizli sütunların gösterilme iki türünü temsil eder"
type: docs
url: /tr/net/aspose.cells/htmlhiddencoldisplaytype/
---
## HtmlHiddenColDisplayType enumeration

HTML'de gizli sütunları gösterme iki türünü temsil eder.

```csharp
public enum HtmlHiddenColDisplayType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Hidden | `0` | HTML sayfasındaki gizli sütunları gizler. |
| Remove | `1` | HTML sayfasındaki gizli sütunları kaldır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlHiddenColDisplayTypeDemo
    {
        public static void HtmlHiddenColDisplayTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // İkinci sütunu gizle
            worksheet.Cells.HideColumn(1);

            // HtmlSaveOptions oluşturun ve HiddenColDisplayType'ı ayarlayın
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Remove;

            // Çalışma kitabını HTML formatında kaydedin
            workbook.Save("HtmlHiddenColDisplayTypeExample.html", saveOptions);

            Console.WriteLine("Workbook saved as HTML with hidden columns removed.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


