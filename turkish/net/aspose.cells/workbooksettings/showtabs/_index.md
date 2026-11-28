---
title: "WorkbookSettings.ShowTabs"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings property. Çalışma kitabı sekmelerinin gösterilip gösterilmeyeceği değerini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/workbooksettings/showtabs/
---
## WorkbookSettings.ShowTabs property

Workbook sekmelerinin görüntülenip görüntülenmeyeceğini belirten bir değeri alır veya ayarlar.

```csharp
public bool ShowTabs { get; set; }
```

### Açıklamalar

Varsayılan değer true'tur.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyShowTabsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Elektronik tablo sekmelerini gizle
            workbook.Settings.ShowTabs = false;
            
            // Çalışma kitabını kaydedin
            workbook.Save("HideTabsDemo.xlsx", SaveFormat.Xlsx);
            
            // Sekmeleri göstermek için başka bir çalışma kitabı oluştur
            Workbook workbook2 = new Workbook();
            
            // Sekmelerin görünür olduğundan emin olun (varsayılan true'dur)
            workbook2.Settings.ShowTabs = true;
            
            // Çalışma kitabını kaydedin
            workbook2.Save("ShowTabsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


