---
title: "WorkbookSettings.WindowTopCM"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. İstemci alanının üst kenarı ile pencerenin üst kenarı arasındaki mesafe, santimetre biriminde"
type: docs
url: /tr/net/aspose.cells/workbooksettings/windowtopcm/
---
## WorkbookSettings.WindowTopCM property

İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, santimetre biriminde.

```csharp
public double WindowTopCM { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopCMDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabı ayarlarına eriş
            WorkbookSettings settings = workbook.Settings;

            // WindowTopCM özelliğini ayarla (üstten santimetre cinsinden konum)
            settings.WindowTopCM = 2.5;

            // Mevcut WindowTopCM değerini göster
            Console.WriteLine("Window Top Position (cm): " + settings.WindowTopCM);

            // Çalışma kitabını kaydedin
            workbook.Save("WindowTopCMDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


