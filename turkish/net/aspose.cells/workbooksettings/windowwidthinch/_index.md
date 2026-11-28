---
title: "WorkbookSettings.WindowWidthInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Pencerenin genişliği inç biriminde"
type: docs
url: /tr/net/aspose.cells/workbooksettings/windowwidthinch/
---
## WorkbookSettings.WindowWidthInch property

Pencerenin genişliği, inç biriminde.

```csharp
public double WindowWidthInch { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthInchDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabı ayarlarına eriş
            WorkbookSettings settings = workbook.Settings;

            // Pencere genişliğini inç cinsinden ayarla
            settings.WindowWidthInch = 10.5;

            // Pencere genişliğini inç cinsinden göster
            Console.WriteLine("Window Width in Inches: " + settings.WindowWidthInch);

            // Çalışma kitabını kaydedin
            workbook.Save("WindowWidthInchDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


