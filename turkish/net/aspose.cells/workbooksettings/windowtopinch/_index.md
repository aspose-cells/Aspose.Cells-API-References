---
title: "WorkbookSettings.WindowTopInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. İstemci alanının üst kenarı ile pencerenin üst kenarı arasındaki mesafe inç biriminde"
type: docs
url: /tr/net/aspose.cells/workbooksettings/windowtopinch/
---
## WorkbookSettings.WindowTopInch property

İstemci alanının üst kenarından pencerenin üst kenarına olan mesafe, inç biriminde.

```csharp
public double WindowTopInch { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopInchDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // WorkbookSettings'a erişin.
            WorkbookSettings settings = workbook.Settings;

            // WindowTopInch özelliğini pencereyi üstten 2 inç konumlandıracak şekilde ayarla
            settings.WindowTopInch = 2.0;

            // Ayarı yazdırarak doğrula
            Console.WriteLine("Window top position (inches): " + settings.WindowTopInch);

            // Çalışma kitabını kaydedin
            workbook.Save("WindowTopInchDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


