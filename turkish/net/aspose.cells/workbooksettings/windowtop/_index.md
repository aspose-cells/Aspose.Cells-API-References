---
title: "WorkbookSettings.WindowTop"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Pencere üst kenarı ile istemci alanının üst kenarı arasındaki mesafe, nokta biriminde"
type: docs
url: /tr/net/aspose.cells/workbooksettings/windowtop/
---
## WorkbookSettings.WindowTop property

İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, nokta biriminde.

```csharp
public double WindowTop { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // WorkbookSettings'a erişin.
            WorkbookSettings settings = workbook.Settings;

            // Pencereyi üstten 100 piksel konumlandırmak için WindowTop özelliğini ayarlayın
            settings.WindowTop = 100;
            
            // WindowTop değerini doğrulayın
            Console.WriteLine("Window top position set to: " + settings.WindowTop);

            // Çalışma kitabını kaydedin
            workbook.Save("WindowTopDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


