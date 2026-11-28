---
title: "CustomRenderSettings.CustomRenderSettings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomRenderSettings yapıcı. Ctor"
type: docs
url: /tr/net/aspose.cells.rendering/customrendersettings/customrendersettings/
---
## CustomRenderSettings constructor

Yapıcı.

```csharp
public CustomRenderSettings()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CustomRenderSettingsMethodSharpctorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Bağlam için bazı veriler ekle
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";

            try
            {
                // CustomRenderSettings sınıfının bir örneğini yapıcı kullanarak oluşturun
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Başarılı yapıcı çağrısının onayını gösterin
                Console.WriteLine("CustomRenderSettings instance created successfully using #ctor");

                // Bir yöntem çağırarak örneğin işlevsel olduğunu gösterin
                float borderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                Console.WriteLine($"Default thin border width: {borderWidth}");

                // Çalışma kitabını kaydedin
                workbook.Save("CustomRenderSettingsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating CustomRenderSettings: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomRenderSettings](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


