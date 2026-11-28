---
title: "AutoFitterOptions.FormatStrategy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFitterOptions özelliği. Biçimlendirme stratejisini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/autofitteroptions/formatstrategy/
---
## AutoFitterOptions.FormatStrategy property

Biçimlendirilmiş stratejiyi alır ve ayarlar.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Açıklamalar

Performans için varsayılan değer CellStyle'dır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyFormatStrategyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ayarlayın ve metni kaydırın
            worksheet.Cells["A1"].PutValue("Sample text for FormatStrategy demo");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            // FormatStrategy ile AutoFitterOptions oluşturun
            AutoFitterOptions options = new AutoFitterOptions
            {
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine
            };

            // Belirtilen seçeneklerle otomatik ayarlamayı uygulayın
            worksheet.AutoFitRows(options);

            // Sonucu kaydet
            workbook.Save("FormatStrategyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


