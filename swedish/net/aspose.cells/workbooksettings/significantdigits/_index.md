---
title: "WorkbookSettings.SignificantDigits"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Hämtar och anger antalet signifikanta siffror. Standardvärdet är SignificantDigits"
type: docs
url: /sv/net/aspose.cells/workbooksettings/significantdigits/
---
## WorkbookSettings.SignificantDigits property

Hämtar och anger antalet signifikanta siffror. Standardvärdet är [`SignificantDigits`](../../cellshelper/significantdigits/).

```csharp
[Obsolete("Use SignificantDigitsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int SignificantDigits { get; set; }
```

### Anmärkningar

Kan nu bara vara 15 eller 17. OBS: Denna medlem är nu föråldrad. Använd istället [`SignificantDigitsType`](../significantdigitstype/). Denna egenskap kommer att tas bort 12 månader senare från och med juni 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySignificantDigitsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempel på numeriska data för att demonstrera signifikanta siffror
            sheet.Cells["A1"].PutValue(123.4567890123456789);
            sheet.Cells["A2"].PutValue(0.000000000123456789);

            // Åtkomst till arbetsboksinställningar
            WorkbookSettings settings = workbook.Settings;

            // Ställ in signifikanta siffror till 15 (maximal precision för double)
            settings.SignificantDigits = 15;

            // Spara arbetsboken för att visa effekten av signifikanta siffror
            workbook.Save("SignificantDigitsDemo.xlsx");

            Console.WriteLine("Workbook saved with SignificantDigits set to 15.");
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


