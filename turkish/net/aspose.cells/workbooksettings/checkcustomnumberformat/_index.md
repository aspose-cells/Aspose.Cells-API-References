---
title: "WorkbookSettings.CheckCustomNumberFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Style.Custom ayarlanırken özel sayı formatının kontrol edilip edilmediğini gösterir"
type: docs
url: /tr/net/aspose.cells/workbooksettings/checkcustomnumberformat/
---
## WorkbookSettings.CheckCustomNumberFormat property

Style.Custom ayarlanırken özel sayı biçiminin kontrol edilip edilmediğini gösterir.

```csharp
public bool CheckCustomNumberFormat { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCheckCustomNumberFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Style style = workbook.CreateStyle();
            
            // Önce geçerli bir özel sayı formatı ayarlayın
            style.Custom = "#,##0.00";
            
            // Katı kontrolü etkinleştir
            workbook.Settings.CheckCustomNumberFormat = true;
            
            try
            {
                // Geçersiz bir özel sayı formatı ayarlamayı deneyin
                style.Custom = "fff @ ggg";
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Error setting custom format: " + ex.Message);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


