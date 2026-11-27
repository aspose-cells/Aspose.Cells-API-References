---
title: "WorkbookSettings.DefaultStyleSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings egenskap. Hämtar inställningarna för standardvärden för stilrelaterade egenskaper för denna arbetsbok."
type: docs
url: /sv/net/aspose.cells/workbooksettings/defaultstylesettings/
---
## WorkbookSettings.DefaultStyleSettings property

Hämtar inställningarna för standardvärden för stilrelaterade egenskaper i denna arbetsbok.

```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```

### Exempel

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDefaultStyleSettingsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Få åtkomst till standardstilinställningarna
            DefaultStyleSettings styleSettings = workbook.Settings.DefaultStyleSettings;

            // Ställ in inbyggt talformatspreferens
            styleSettings.BuiltInPreference = true;

            // Ställ in kultur för talformatering
            workbook.Settings.CultureInfo = new CultureInfo("en-US");

            // Få åtkomst till celler och tillämpa formatering
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ange värden och format
            cells["A1"].PutValue(1234.56);
            cells["A1"].GetStyle().Number = 4; // Currency format

            cells["B1"].PutValue(0.456);
            cells["B1"].GetStyle().Number = 2; // Percentage format

            cells["C1"].PutValue(DateTime.Now);
            cells["C1"].GetStyle().Number = 22; // Short date format

            // Spara arbetsboken
            workbook.Save("DefaultStyleSettingsDemo.xlsx");
        }
    }
}
```

### Se även

* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


