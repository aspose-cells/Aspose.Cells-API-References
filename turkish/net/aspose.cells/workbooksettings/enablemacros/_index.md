---
title: "WorkbookSettings.EnableMacros"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Makroları etkinleştir"
type: docs
url: /tr/net/aspose.cells/workbooksettings/enablemacros/
---
## WorkbookSettings.EnableMacros property

Makroları etkinleştir;

```csharp
public bool EnableMacros { get; set; }
```

### Açıklamalar

Şimdi, bir çalışma kitabında bir çalışma sayfasını başka bir çalışma sayfasına kopyalarken yalnızca çalışır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyEnableMacrosDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = wb.Worksheets[0];
            
            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("Macro Test");
            
            // EnableMacros özelliğini gösterin
            Console.WriteLine("Initial EnableMacros value: " + wb.Settings.EnableMacros);
            
            // Makroları devre dışı bırak
            wb.Settings.EnableMacros = false;
            Console.WriteLine("After disabling macros: " + wb.Settings.EnableMacros);
            
            // Makroları etkinleştir
            wb.Settings.EnableMacros = true;
            Console.WriteLine("After enabling macros: " + wb.Settings.EnableMacros);
            
            // Çalışma kitabını kaydedin
            wb.Save("EnableMacrosDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


