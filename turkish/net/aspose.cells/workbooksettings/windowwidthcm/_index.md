---
title: "WorkbookSettings.WindowWidthCM"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Pencerenin genişliği santimetre biriminde"
type: docs
url: /tr/net/aspose.cells/workbooksettings/windowwidthcm/
---
## WorkbookSettings.WindowWidthCM property

Pencerenin genişliği, santimetre biriminde.

```csharp
public double WindowWidthCM { get; set; }
```

### Örnekler

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthCMDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // WorkbookSettings'a erişin.
            WorkbookSettings settings = workbook.Settings;
            
            // WindowWidthCM özelliğini ayarlayın (20.32 cm = ~8 inç)
            settings.WindowWidthCM = 20.32;
            
            // Ayarı yazdırarak doğrula
            Console.WriteLine("Window Width in Centimeters: " + settings.WindowWidthCM);
            
            // Çalışma kitabını kaydedin
            workbook.Save("WindowWidthCMDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


