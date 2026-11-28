---
title: "WorkbookSettings.WindowLeftInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe. İnç biriminde"
type: docs
url: /tr/net/aspose.cells/workbooksettings/windowleftinch/
---
## WorkbookSettings.WindowLeftInch property

İstemci alanının sol kenarından pencerenin sol kenarına olan mesafe, inç biriminde.

```csharp
public double WindowLeftInch { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftInchDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // WorkbookSettings'a erişin.
            WorkbookSettings settings = workbook.Settings;

            // WindowLeftInch özelliğini ayarlayın
            settings.WindowLeftInch = 1.5; // Position window 1.5 inches from left edge of screen

            // Çalışma kitabının işlevsel olduğunu göstermek için bazı örnek veriler ekleyin
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Window Position Demo");
            sheet.Cells["A2"].PutValue($"Window left position: {settings.WindowLeftInch} inches");

            // Çalışma kitabını kaydedin
            workbook.Save("WindowLeftInchDemo.xlsx");

            Console.WriteLine("Workbook saved with WindowLeftInch = " + settings.WindowLeftInch);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


