---
title: "WorkbookSettings.NumberDecimalSeparator"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Sayısal değerlerin biçimlendirilmesi/ayrıştırılması için ondalık ayırıcıyı alır veya ayarlar. Varsayılan, geçerli bölgenin ondalık ayırıcısıdır"
type: docs
url: /tr/net/aspose.cells/workbooksettings/numberdecimalseparator/
---
## WorkbookSettings.NumberDecimalSeparator property

Sayısal değerlerin biçimlendirilmesi/ayrıştırılması için ondalık ayırıcıyı alır veya ayarlar. Varsayılan, geçerli Bölgenin ondalık ayırıcısıdır.

```csharp
public char NumberDecimalSeparator { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyNumberDecimalSeparatorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.NumberDecimalSeparator = ',';
            wb.Settings.NumberGroupSeparator = '.';
            
            Style style = wb.CreateStyle();
            style.Custom = "#,##0.00";
            
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            cell.PutValue(12345.6798);
            cell.SetStyle(style);
            
            Console.WriteLine("Formatted value: " + cell.StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


