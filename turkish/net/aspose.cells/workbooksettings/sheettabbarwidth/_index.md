---
title: "WorkbookSettings.SheetTabBarWidth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Çalışma sayfası sekme çubuğunun genişliği, pencere genişliğinin 1/1000'i cinsinden"
type: docs
url: /tr/net/aspose.cells/workbooksettings/sheettabbarwidth/
---
## WorkbookSettings.SheetTabBarWidth property

Çalışma sayfası sekme çubuğunun genişliği (pencere genişliğinin 1/1000'i cinsinden).

```csharp
public int SheetTabBarWidth { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySheetTabBarWidthDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // SheetTabBarWidth özelliğini ayarlayın
            workbook.Settings.SheetTabBarWidth = 1000;
            
            // SheetTabBarWidth değerini al ve görüntüle
            Console.WriteLine("SheetTabBarWidth: " + workbook.Settings.SheetTabBarWidth);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


