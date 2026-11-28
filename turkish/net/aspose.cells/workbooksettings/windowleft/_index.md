---
title: "WorkbookSettings.WindowLeft"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe, nokta biriminde"
type: docs
url: /tr/net/aspose.cells/workbooksettings/windowleft/
---
## WorkbookSettings.WindowLeft property

İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe, nokta biriminde.

```csharp
public double WindowLeft { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // WorkbookSettings'a erişin.
            WorkbookSettings settings = workbook.Settings;

            // WindowLeft özelliğini ayarlayarak pencereyi soldan 100 piksel konumlandır
            settings.WindowLeft = 100;

            // Demonstrasyon için diğer pencere özelliklerini ayarla
            settings.WindowTop = 50;
            settings.WindowWidth = 800;
            settings.WindowHeight = 600;

            // Çalışma sayfasına örnek veri ekle
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Window Position Demo");
            sheet.Cells["A2"].PutValue($"Left: {settings.WindowLeft}px");
            sheet.Cells["A3"].PutValue($"Top: {settings.WindowTop}px");

            // Çalışma kitabını kaydedin
            workbook.Save("WindowPositionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


