---
title: "Enum HtmlHiddenRowDisplayType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "**Aspose.Cells.HtmlHiddenRowDisplayType** enum. HTML'de gizli satırların gösterilmesinin iki tipini temsil eder"
type: docs
url: /tr/net/aspose.cells/htmlhiddenrowdisplaytype/
---
## HtmlHiddenRowDisplayType enumeration

HTML'de gizli satırları gösterme iki türünü temsil eder.

```csharp
public enum HtmlHiddenRowDisplayType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Hidden | `0` | HTML sayfasındaki gizli satırları gizle. |
| Remove | `1` | HTML sayfasındaki gizli satırları kaldır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlHiddenRowDisplayTypeDemo
    {
        public static void HtmlHiddenRowDisplayTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            worksheet.Cells["A1"].PutValue("Visible Row");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Another Visible Row");

            // İkinci satırı gizle
            worksheet.Cells.HideRow(1);

            // HtmlSaveOptions oluştur ve HiddenRowDisplayType'ı ayarla
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden; // or HtmlHiddenRowDisplayType.Remove

            // Çalışma kitabını HTML formatında kaydedin
            workbook.Save("HtmlHiddenRowDisplayTypeExample.html", saveOptions);

            Console.WriteLine("Workbook saved as HTML with hidden row display type.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


