---
title: "WorkbookSettings.WindowLeftCM"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe. Santimetre biriminde"
type: docs
url: /tr/net/aspose.cells/workbooksettings/windowleftcm/
---
## WorkbookSettings.WindowLeftCM property

İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe, santimetre biriminde.

```csharp
public double WindowLeftCM { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftCMDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // WorkbookSettings'a erişin.
            WorkbookSettings settings = workbook.Settings;

            // WindowLeftCM özelliğini ayarlayın (ekranın sol kenarından santimetre cinsinden mesafe)
            settings.WindowLeftCM = 2.54; // 1 inch = 2.54 cm

            // Ayarı yazdırarak doğrula
            Console.WriteLine("WindowLeftCM: " + settings.WindowLeftCM);

            // Çalışma kitabını kaydedin
            workbook.Save("WindowLeftCMDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


