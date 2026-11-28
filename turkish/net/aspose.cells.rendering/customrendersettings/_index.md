---
title: "Sınıf CustomRenderSettings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.CustomRenderSettings sınıfı. İşleme sırasında özel ayarları temsil eder"
type: docs
url: /tr/net/aspose.cells.rendering/customrendersettings/
---
## CustomRenderSettings class

Oluşturma sırasında özel ayarları temsil eder.

```csharp
public class CustomRenderSettings
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [CustomRenderSettings](customrendersettings/)() | Yapıcı. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| virtual [GetCellBorderWidth](../../aspose.cells.rendering/customrendersettings/getcellborderwidth/)(CellBorderType) | Hücre kenarlık genişliğini kenarlık türüne göre belirtir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassCustomRenderSettingsDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";
            worksheet.Cells["A2"].Value = "Border Width Test";

            try
            {
                // Varsayılan yapıcıyı kullanarak CustomRenderSettings örneği oluşturun
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // GetCellBorderWidth yöntemini farklı kenarlık türleriyle gösterin
                float thinWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                float thickWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thick);
                float dashedWidth = renderSettings.GetCellBorderWidth(CellBorderType.Dashed);

                // Sonuçları görüntüleyin
                Console.WriteLine($"Thin border width: {thinWidth}");
                Console.WriteLine($"Thick border width: {thickWidth}");
                Console.WriteLine($"Dashed border width: {dashedWidth}");

                // Çalışma kitabını kaydedin
                workbook.Save("CustomRenderSettingsDemo.xlsx");
                Console.WriteLine("CustomRenderSettings demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in CustomRenderSettings demonstration: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


