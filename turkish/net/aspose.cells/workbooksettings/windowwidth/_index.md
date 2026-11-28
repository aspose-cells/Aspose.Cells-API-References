---
title: "WorkbookSettings.WindowWidth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings property. Pencerenin genişliği nokta biriminde"
type: docs
url: /tr/net/aspose.cells/workbooksettings/windowwidth/
---
## WorkbookSettings.WindowWidth property

Pencerenin genişliği, nokta biriminde.

```csharp
public double WindowWidth { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // WorkbookSettings'a erişin.
            WorkbookSettings settings = workbook.Settings;
            
            // WindowWidth özelliğini ayarlayın
            settings.WindowWidth = 800;
            
            // WindowWidth değerini doğrula
            Console.WriteLine("Window Width set to: " + settings.WindowWidth);
            
            // Çalışma kitabını kaydedin
            workbook.Save("WindowWidthDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


