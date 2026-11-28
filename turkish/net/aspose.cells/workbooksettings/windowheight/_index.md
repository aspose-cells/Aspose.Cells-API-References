---
title: "WorkbookSettings.WindowHeight"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Pencerenin yüksekliği nokta biriminde"
type: docs
url: /tr/net/aspose.cells/workbooksettings/windowheight/
---
## WorkbookSettings.WindowHeight property

Pencerenin yüksekliği, nokta biriminde.

```csharp
public double WindowHeight { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // WorkbookSettings'a erişin.
            WorkbookSettings settings = workbook.Settings;
            
            // WindowHeight özelliğini ayarlayın
            settings.WindowHeight = 600;
            
            // WindowHeight değerini doğrulayın
            Console.WriteLine("Window Height set to: " + settings.WindowHeight);
            
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


