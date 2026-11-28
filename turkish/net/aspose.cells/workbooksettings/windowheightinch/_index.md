---
title: "WorkbookSettings.WindowHeightInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Pencerenin yüksekliği inç biriminde"
type: docs
url: /tr/net/aspose.cells/workbooksettings/windowheightinch/
---
## WorkbookSettings.WindowHeightInch property

Pencerenin yüksekliği, inç biriminde.

```csharp
public double WindowHeightInch { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightInchDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabı ayarlarına eriş
            WorkbookSettings settings = workbook.Settings;

            // Pencere yüksekliğini inç olarak ayarla
            settings.WindowHeightInch = 5.5;

            // Pencere yüksekliğini inç olarak göster
            Console.WriteLine("Window Height in Inches: " + settings.WindowHeightInch);

            // Çalışma kitabını kaydedin
            workbook.Save("WindowHeightInchDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


