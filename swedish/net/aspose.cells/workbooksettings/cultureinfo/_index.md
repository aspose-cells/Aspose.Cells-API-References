---
title: "WorkbookSettings.CultureInfo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings‑egenskap. Hämtar eller anger systemets kulturinformation"
type: docs
url: /sv/net/aspose.cells/workbooksettings/cultureinfo/
---
## WorkbookSettings.CultureInfo property

Hämtar eller anger systemets kulturinformation.

```csharp
public CultureInfo CultureInfo { get; set; }
```

### Anmärkningar

Returnerar null om kulturinformationen inte är angiven och [`Region`](../region/) inte är angiven.

### Exempel

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
            // Skapa en arbetsbok
            Workbook wb = new Workbook();
            
            // Ange region till Frankrike för att demonstrera ändringar i CultureInfo
            wb.Settings.Region = CountryCode.France;
            
            // Hämta grupperingstecknet från fransk kultur
            string groupSep = wb.Settings.CultureInfo.NumberFormat.NumberGroupSeparator;
            Console.WriteLine($"French group separator: '{groupSep}'");
            
            // Skapa en stil med anpassat format och visa kulturanpassat format
            Style style = wb.CreateStyle();
            style.Custom = "#,##0.00_ ;-#,##0.00";
            Console.WriteLine($"Culture-adjusted custom format: {style.CultureCustom}");
            
            // Demonstrera talformatering med fransk kultur
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

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


