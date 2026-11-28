---
title: "WorkbookSettings.SmartTagOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Akıllı etiketin seçeneklerini alır"
type: docs
url: /tr/net/aspose.cells/workbooksettings/smarttagoptions/
---
## WorkbookSettings.SmartTagOptions property

Akıllı etiketin seçeneklerini alır.

```csharp
public SmartTagOptions SmartTagOptions { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySmartTagOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();

                // Çalışma kitabı ayarlarına erişin
                WorkbookSettings settings = workbook.Settings;

                // SmartTagOptions özelliğini oku
                var smartTagOptions = settings.SmartTagOptions;

                // SmartTagOptions örneği hakkında bilgileri göster
                Console.WriteLine("SmartTagOptions instance type: " + smartTagOptions.GetType().FullName);

                // İsteğe bağlı olarak, varsayılan durumu ToString() ile inceleyebilirsiniz
                Console.WriteLine("SmartTagOptions details: " + smartTagOptions.ToString());

                // Çalışma kitabını kaydet (dosya varsayılan ayarları içerecek)
                workbook.Save("SmartTagOptionsDemo.xlsx");
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

* class [SmartTagOptions](../../../aspose.cells.markup/smarttagoptions/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


