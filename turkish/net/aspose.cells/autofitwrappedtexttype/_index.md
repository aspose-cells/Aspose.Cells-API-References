---
title: "Enum AutoFitWrappedTextType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.AutoFitWrappedTextType enum. Sarılmış metnin otomatik sığdırma tipini temsil eder"
type: docs
url: /tr/net/aspose.cells/autofitwrappedtexttype/
---
## AutoFitWrappedTextType enumeration

Satır içi metnin otomatik sığdırma türünü temsil eder.

```csharp
public enum AutoFitWrappedTextType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Default | `0` | MS Excel gibi çalışır. |
| Paragraph | `1` | En uzun paragrafla genişliği otomatik olarak sığdır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitWrappedTextTypeDemo
    {
        public static void AutoFitWrappedTextTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("This is a sample text that will be wrapped and auto-fitted.\r\n This is a sample text that will be wrapped and auto-fitted. This is a sample text that will be wrapped and auto-fitted. This is a sample text that will be wrapped and auto-fitted.");
            worksheet.Cells["A5"].PutValue("Another sample text to demonstrate \r\n auto-fitting wrapped text. Another sample text to demonstrate auto-fitting wrapped text.\r\n Another sample text to demonstrate auto-fitting wrapped text. Another sample text to demonstrate auto-fitting wrapped text.");

            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            Style style2 = worksheet.Cells["A5"].GetStyle();
            style2.IsTextWrapped = true;
            worksheet.Cells["A5"].SetStyle(style);

            // A1:F3 aralığını oluştur
            Range range = worksheet.Cells.CreateRange(0, 0, 3, 6);
            // Hücreleri birleştir
            range.Merge();

            // A4:F6 aralığını oluştur
            Range range2 = worksheet.Cells.CreateRange(4, 0, 3, 6);
            // Hücreleri birleştir
            range2.Merge();

            // AutoFitterOptions oluştur ve AutoFitWrappedTextType'ı ayarla
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph;

            // Belirtilen seçeneklerle satırları otomatik sığdır.
            worksheet.AutoFitRows(options);

            // Çalışma kitabını kaydedin
            workbook.Save("AutoFitWrappedTextTypeExample.xlsx");
            workbook.Save("AutoFitWrappedTextTypeExample.pdf");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


