---
title: "LoadOptions.AutoFitterOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Otomatik sığdırma seçeneklerini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/loadoptions/autofitteroptions/
---
## LoadOptions.AutoFitterOptions property

Otomatik sığdırma seçeneklerini alır ve ayarlar

```csharp
public AutoFitterOptions AutoFitterOptions { get; set; }
```

### Açıklamalar

Şu anda yalnızca xlsx, spreadsheetML dosyaları için.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // AutoFitterOptions oluştur ve özellikleri ayarla
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCells = true;
            options.OnlyAuto = false;

            // LoadOptions oluştur ve AutoFitterOptions atayın
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.AutoFitterOptions = options;

            // Belirtilen seçeneklerle çalışma kitabını yükle
            Workbook workbook = new Workbook("example.xlsx", loadOptions);

            // Satır yüksekliğini alarak otomatik sığdırmayı göster
            double rowHeight = workbook.Worksheets[0].Cells.GetRowHeight(0);
            Console.WriteLine("Row height after auto-fitting: " + rowHeight);
        }
    }
}
```

### Ayrıca Bakınız

* class [AutoFitterOptions](../../autofitteroptions/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


