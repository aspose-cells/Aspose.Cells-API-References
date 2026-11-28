---
title: "WorkbookSettings.Date1904"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Çalışma kitabının 1904 tarih sistemini kullanıp kullanmadığını temsil eden bir değeri alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/workbooksettings/date1904/
---
## WorkbookSettings.Date1904 property

Çalışma kitabının 1904 tarih sistemini kullanıp kullanmadığını temsil eden bir değeri alır veya ayarlar.

```csharp
public bool Date1904 { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDate1904Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Date1904 = true;

            Worksheet sheet = wb.Worksheets[0];
            Cell cell = sheet.Cells[0, 0];
            
            // Date1904 ile negatif zamanı göster
            Style style = cell.GetStyle();
            style.Custom = "h:mm";
            cell.SetStyle(style);
            cell.PutValue(-0.0736111111111112);
            Console.WriteLine("Negative time value: " + cell.DisplayStringValue);

            // Date1904 ile negatif tarihi göster
            style = cell.GetStyle();
            style.Custom = "mm/dd/yyyy h:mm:ss";
            cell.SetStyle(style);
            cell.PutValue(-42389.47075706);
            Console.WriteLine("Negative date value: " + cell.DisplayStringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


