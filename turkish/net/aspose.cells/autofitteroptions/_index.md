---
title: "AutoFitterOptions sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.AutoFitterOptions sınıfı. Tüm otomatik sığdırma seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/autofitteroptions/
---
## AutoFitterOptions class

Tüm otomatik sığdırma seçeneklerini temsil eder.

```csharp
public class AutoFitterOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [AutoFitterOptions](autofitteroptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AutoFitMergedCells](../../aspose.cells/autofitteroptions/autofitmergedcells/) { get; set; } | (**Obsolete.**) Bir satırda hücreler birleştirildiğinde satır yüksekliğinin otomatik ayarlanıp ayarlanmayacağını gösterir. Varsayılan değer false'dur. |
| [AutoFitMergedCellsType](../../aspose.cells/autofitteroptions/autofitmergedcellstype/) { get; set; } | Birleştirilmiş hücrelerin satır yüksekliğinin otomatik ayarlanma türünü alır ve ayarlar. |
| [AutoFitWrappedTextType](../../aspose.cells/autofitteroptions/autofitwrappedtexttype/) { get; set; } | Satır sonu ile sarılmış metnin otomatik ayarlanma türünü alır ve ayarlar. |
| [DefaultEditLanguage](../../aspose.cells/autofitteroptions/defaulteditlanguage/) { get; set; } | Varsayılan düzenleme dilini alır veya ayarlar. |
| [FormatStrategy](../../aspose.cells/autofitteroptions/formatstrategy/) { get; set; } | Biçimlendirilmiş stratejiyi alır ve ayarlar. |
| [ForRendering](../../aspose.cells/autofitteroptions/forrendering/) { get; set; } | Render amacı için uyumlu olup olmadığını gösterir. |
| [IgnoreHidden](../../aspose.cells/autofitteroptions/ignorehidden/) { get; set; } | Gizli satırları/sütunları yok sayar. |
| [MaxRowHeight](../../aspose.cells/autofitteroptions/maxrowheight/) { get; set; } | Satırları otomatik ayarlarken maksimum satır yüksekliğini (Point biriminde) alır ve ayarlar. |
| [OnlyAuto](../../aspose.cells/autofitteroptions/onlyauto/) { get; set; } | Yüksekliği özelleştirilmemiş satırların yalnızca ayarlanıp ayarlanmayacağını gösterir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitterOptionsDemo
    {
        public static void AutoFitterOptionsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("This is a sample text that will be wrapped and autofitted.");

            Style style = worksheet.Cells["A1"].GetStyle();

            style.IsTextWrapped = true;

            worksheet.Cells["A1"].SetStyle(style);

            // A1:B2 aralığını oluştur
            Range range = worksheet.Cells.CreateRange(0, 0, 2, 2);

            // Hücreleri birleştir
            range.Merge();

            // AutoFitterOptions sınıfının bir örneğini oluştur.
            AutoFitterOptions options = new AutoFitterOptions
            {
                DefaultEditLanguage = DefaultEditLanguage.English,
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                OnlyAuto = true,
                IgnoreHidden = true,
                MaxRowHeight = 50.0,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                ForRendering = true
            };

            // Belirtilen seçeneklerle otomatik satır sığdırmayı uygulayın
            worksheet.AutoFitRows(options);

            // Çalışma kitabını kaydedin
            workbook.Save("AutoFitterOptionsExample.xlsx");
            workbook.Save("AutoFitterOptionsExample.pdf");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


