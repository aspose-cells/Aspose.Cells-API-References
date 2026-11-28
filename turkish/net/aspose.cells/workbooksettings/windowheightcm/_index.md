---
title: "WorkbookSettings.WindowHeightCM"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Pencerenin yüksekliği santimetre biriminde"
type: docs
url: /tr/net/aspose.cells/workbooksettings/windowheightcm/
---
## WorkbookSettings.WindowHeightCM property

Pencerenin yüksekliği, santimetre biriminde.

```csharp
public double WindowHeightCM { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightCMDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabı ayarlarına eriş
            WorkbookSettings settings = workbook.Settings;

            // WindowHeightCM özelliğini ayarlayın
            settings.WindowHeightCM = 15.5;

            // Ayarlanan değeri görüntüleyin
            Console.WriteLine("Window Height in Centimeters: " + settings.WindowHeightCM);

            // Çalışma kitabını kaydedin
            workbook.Save("WindowHeightDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


