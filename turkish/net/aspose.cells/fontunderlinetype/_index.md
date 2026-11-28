---
title: "Enum FontUnderlineType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FontUnderlineType enum. Yazı tipi alt çizgi türlerini sıralar"
type: docs
url: /tr/net/aspose.cells/fontunderlinetype/
---
## FontUnderlineType enumeration

Yazı tipi alt çizgi türlerini sıralar.

```csharp
public enum FontUnderlineType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Alt çizgi yoktur. |
| Single | `1` | Tek alt çizgi temsil eder. |
| Double | `2` | Çift alt çizgi temsil eder. |
| Accounting | `3` | Tek muhasebe alt çizgisi temsil eder. |
| DoubleAccounting | `4` | Çift muhasebe alt çizgisi temsil eder. |
| Dash | `5` | Kesikli alt çizgi temsil eder |
| DashDotDotHeavy | `6` | Kalın Kesik-Nokta-Nokta alt çizgi temsil eder |
| DashDotHeavy | `7` | Kalın Kesik-Nokta alt çizgi temsil eder |
| DashedHeavy | `8` | Kalın Kesikli alt çizgi temsil eder |
| DashLong | `9` | Uzun Kesikli alt çizgi temsil eder |
| DashLongHeavy | `10` | Kalın Uzun Kesikli alt çizgi temsil eder |
| DotDash | `11` | Kesik-Nokta alt çizgi temsil eder |
| DotDotDash | `12` | Kesik-Nokta-Nokta alt çizgi temsil eder |
| Dotted | `13` | Noktalı alt çizgi temsil eder |
| DottedHeavy | `14` | Kalın Noktalı alt çizgi temsil eder |
| Heavy | `15` | Kalın alt çizgi temsil eder |
| Wave | `16` | Dalga Altı Çizgiyi temsil eder |
| WavyDouble | `17` | Çift Dalga Altı Çizgiyi temsil eder |
| WavyHeavy | `18` | Kalın Dalga Altı Çizgiyi temsil eder |
| Words | `19` | Boşluk olmayan karakterlerin altını çizer. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontUnderlineTypeDemo
    {
        public static void FontUnderlineTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasının referansını alın.
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasından "A1" hücresine erişme
            Cell cell = worksheet.Cells["A1"];
            
            // "A1" hücresine bir değer ekleme
            cell.PutValue("Hello Aspose!");

            // Hücrenin stilini al
            Style style = cell.GetStyle();
            
            // Yazı tipi altı çizgi tipini tek altı çizgi olarak ayarla
            style.Font.Underline = FontUnderlineType.Single;
            
            // Stili hücreye uygulayın
            cell.SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("FontUnderlineTypeExample.xlsx");
            workbook.Save("FontUnderlineTypeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


