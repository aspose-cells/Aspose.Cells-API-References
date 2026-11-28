---
title: "MsoFillFormatHelper.IsVisible"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoFillFormatHelper özelliği. Doldurma olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/msofillformathelper/isvisible/
---
## MsoFillFormatHelper.IsVisible property

Dolgu olup olmadığını gösterir.

```csharp
public bool IsVisible { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örneği anlamlı kılmak için bir etiket ekle
            worksheet.Cells["A1"].Value = "IsVisible Property Demo";

            try
            {
                // Yansıma kullanarak MsoFillFormatHelper örneği oluştur (herkese açık yapıcı yok)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Varsayılan IsVisible değerini gösterin
                Console.WriteLine($"Default IsVisible: {fillHelper.IsVisible}");

                // IsVisible'ı true olarak ayarlayın
                fillHelper.IsVisible = true;
                Console.WriteLine($"After setting to true: {fillHelper.IsVisible}");

                // IsVisible'ı false olarak ayarlayın
                fillHelper.IsVisible = false;
                Console.WriteLine($"After setting to false: {fillHelper.IsVisible}");

                // Mevcut IsVisible değerini okuyun
                bool isVisible = fillHelper.IsVisible;
                Console.WriteLine($"Current IsVisible value: {isVisible}");

                // Başarılı yürütmeyi göstermek için çalışma kitabını kaydet.
                workbook.Save("IsVisibleDemo.xlsx");

                Console.WriteLine("IsVisible property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during IsVisible demo: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


