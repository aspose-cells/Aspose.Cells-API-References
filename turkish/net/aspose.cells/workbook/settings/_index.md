---
title: "Workbook.Settings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Çalışma kitabı ayarlarını temsil eder"
type: docs
url: /tr/net/aspose.cells/workbook/settings/
---
## Workbook.Settings property

Çalışma kitabı ayarlarını temsil eder.

```csharp
public WorkbookSettings Settings { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertySettingsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Ayarları erişin ve değiştirin
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 30;
            workbook.Settings.FormulaSettings.MaxChange = 0.1;

            // Ayarları doğrulayın
            Console.WriteLine("Iterative Calculation Enabled: " + 
                workbook.Settings.FormulaSettings.EnableIterativeCalculation);
            Console.WriteLine("Max Iterations: " + 
                workbook.Settings.FormulaSettings.MaxIteration);
            Console.WriteLine("Max Change: " + 
                workbook.Settings.FormulaSettings.MaxChange);

            // Çalışma kitabını kaydedin
            workbook.Save("WorkbookSettingsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../../workbooksettings/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


