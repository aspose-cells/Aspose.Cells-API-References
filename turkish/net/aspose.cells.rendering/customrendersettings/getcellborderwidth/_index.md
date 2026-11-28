---
title: "CustomRenderSettings.GetCellBorderWidth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomRenderSettings yöntemi. Hücre kenar genişliğini kenar tipine göre belirtir"
type: docs
url: /tr/net/aspose.cells.rendering/customrendersettings/getcellborderwidth/
---
## CustomRenderSettings.GetCellBorderWidth method

Hücre kenarlık genişliğini kenarlık türüne göre belirtir.

```csharp
public virtual float GetCellBorderWidth(CellBorderType borderType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| borderType | CellBorderType | hücre kenar tipi |

### Dönüş Değeri

hücre kenar genişliği

### Açıklamalar

Negatif değerler yok sayılacaktır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CustomRenderSettingsMethodGetCellBorderWidthWithCellBorderTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Bağlam için bazı veriler ekle
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // CustomRenderSettings sınıfının bir örneğini oluşturun
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // GetCellBorderWidth yöntemini farklı kenar tipleriyle çağırın
                float thinBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                float thickBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thick);
                float dashedBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Dashed);

                // Sonuçları görüntüleyin
                Console.WriteLine($"Thin border width: {thinBorderWidth}");
                Console.WriteLine($"Thick border width: {thickBorderWidth}");
                Console.WriteLine($"Dashed border width: {dashedBorderWidth}");

                // Çalışma kitabını kaydedin
                workbook.Save("GetCellBorderWidthDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [CellBorderType](../../../aspose.cells/cellbordertype/)
* class [CustomRenderSettings](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


