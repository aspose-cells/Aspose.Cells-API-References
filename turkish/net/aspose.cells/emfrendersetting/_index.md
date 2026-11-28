---
title: "Enum EmfRenderSetting"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.EmfRenderSetting enum. Emf metafilesinin işlenmesi için ayar"
type: docs
url: /tr/net/aspose.cells/emfrendersetting/
---
## EmfRenderSetting enumeration

Emf metafilesinin render edilmesi için ayar.

```csharp
public enum EmfRenderSetting
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| EmfOnly | `0` | Yalnızca Emf kayıtlarını işler. |
| EmfPlusPrefer | `1` | EmfPlus kayıtlarını işlemeyi tercih eder. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class CellsClassEmfRenderSettingDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("EMF Render Setting Demo");
            worksheet.Cells["A2"].PutValue("Using EmfOnly setting");

            // EMF işleme ayarıyla görüntü seçenekleri oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                EmfRenderSetting = EmfRenderSetting.EmfOnly
            };

            // Seçeneklerle bir sayfa işleme oluştur
            SheetRender render = new SheetRender(worksheet, options);

            // İlk sayfayı EMF görüntüsü olarak kaydet
            render.ToImage(0, "EmfRenderSettingDemo.emf");

            Console.WriteLine("EMF file created successfully with EmfOnly setting.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


