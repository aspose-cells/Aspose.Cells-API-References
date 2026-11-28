---
title: "WorkbookSettings.CultureInfo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Sistem kültür bilgisini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/workbooksettings/cultureinfo/
---
## WorkbookSettings.CultureInfo property

Sistem kültür bilgilerini alır veya ayarlar.

```csharp
public CultureInfo CultureInfo { get; set; }
```

### Açıklamalar

Kültür bilgisi ayarlanmamış ve [`Region`](../region/) ayarlanmamışsa null döndürür.

### Örnekler

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCultureInfoDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // CultureInfo değişikliklerini göstermek için bölgeyi Fransa olarak ayarlayın
            wb.Settings.Region = CountryCode.France;
            
            // Fransız kültüründen grup ayırıcıyı alın
            string groupSep = wb.Settings.CultureInfo.NumberFormat.NumberGroupSeparator;
            Console.WriteLine($"French group separator: '{groupSep}'");
            
            // Özel biçimle bir stil oluşturun ve kültüre göre ayarlanmış biçimi gösterin
            Style style = wb.CreateStyle();
            style.Custom = "#,##0.00_ ;-#,##0.00";
            Console.WriteLine($"Culture-adjusted custom format: {style.CultureCustom}");
            
            // Fransız kültürüyle sayı biçimlendirmeyi gösterin
            Worksheet sheet = wb.Worksheets[0];
            Cell cell = sheet.Cells["A1"];
            cell.PutValue(123456.78);
            cell.SetStyle(style);
            style.Custom = "# ###,00 €";
            
            Console.WriteLine($"Formatted value: {cell.StringValue}");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


