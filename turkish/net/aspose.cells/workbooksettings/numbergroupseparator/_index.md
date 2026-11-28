---
title: "WorkbookSettings.NumberGroupSeparator"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Sayısal değerlerde ondalık noktasının solundaki basamak gruplarını ayıran karakteri alır veya ayarlar. Varsayılan, geçerli Bölgenin grup ayırıcı karakteridir."
type: docs
url: /tr/net/aspose.cells/workbooksettings/numbergroupseparator/
---
## WorkbookSettings.NumberGroupSeparator property

Sayısal değerlerde ondalık noktasının solundaki rakam gruplarını ayıran karakteri alır veya ayarlar. Varsayılan, geçerli Bölgenin grup ayırıcıdır.

```csharp
public char NumberGroupSeparator { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyNumberGroupSeparatorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
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


