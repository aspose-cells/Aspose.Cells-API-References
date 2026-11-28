---
title: "WorkbookSettings.IsHidden"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Bu çalışma kitabının gizli olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/workbooksettings/ishidden/
---
## WorkbookSettings.IsHidden property

Bu çalışma kitabının gizli olup olmadığını gösterir.

```csharp
public bool IsHidden { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabı ayarlarına eriş
            WorkbookSettings settings = workbook.Settings;

            // IsHidden özelliğini true olarak ayarla
            settings.IsHidden = true;
            Console.WriteLine("Workbook is hidden: " + settings.IsHidden);

            // Çalışma kitabını kaydedin
            workbook.Save("WorkbookSettings_IsHidden_True.xlsx");

            // Başka bir çalışma kitabı oluştur
            Workbook workbook2 = new Workbook();

            // Çalışma kitabı ayarlarına eriş
            WorkbookSettings settings2 = workbook2.Settings;

            // IsHidden özelliğini false (varsayılan) olarak ayarla
            settings2.IsHidden = false;
            Console.WriteLine("Workbook is hidden: " + settings2.IsHidden);

            // Çalışma kitabını kaydedin
            workbook2.Save("WorkbookSettings_IsHidden_False.xlsx");

            // Kaydedilen çalışma kitaplarını yükle ve kontrol et
            Workbook loadedWorkbook1 = new Workbook("WorkbookSettings_IsHidden_True.xlsx");
            Console.WriteLine("Loaded workbook1 is hidden: " + loadedWorkbook1.Settings.IsHidden);

            Workbook loadedWorkbook2 = new Workbook("WorkbookSettings_IsHidden_False.xlsx");
            Console.WriteLine("Loaded workbook2 is hidden: " + loadedWorkbook2.Settings.IsHidden);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


