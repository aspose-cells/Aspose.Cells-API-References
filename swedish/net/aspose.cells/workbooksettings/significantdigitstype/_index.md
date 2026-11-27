---
title: "WorkbookSettings.SignificantDigitsType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings‑egenskap. Hämtar och anger typen av signifikanta siffror för utskrift av numeriska värden i denna arbetsbok. Standardvärdet är SignificantDigitsType"
type: docs
url: /sv/net/aspose.cells/workbooksettings/significantdigitstype/
---
## WorkbookSettings.SignificantDigitsType property

Hämtar och anger typen av signifikanta siffror för utskrift av numeriska värden i denna arbetsbok. Standardvärdet är [`SignificantDigitsType`](../../cellshelper/significantdigitstype/).

```csharp
public SignificantDigitsType SignificantDigitsType { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookSettingsPropertySignificantDigitsTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Visa det aktuella värdet för SignificantDigitsType
            Console.WriteLine("Current SignificantDigitsType: " + settings.SignificantDigitsType);

            // Demonstrera inställning av olika SignificantDigitsType‑värden
            settings.SignificantDigitsType = SignificantDigitsType.Digits15;
            Console.WriteLine("After setting to Digits15: " + settings.SignificantDigitsType);

            settings.SignificantDigitsType = SignificantDigitsType.G17;
            Console.WriteLine("After setting to G17: " + settings.SignificantDigitsType);

            settings.SignificantDigitsType = SignificantDigitsType.Rounding17;
            Console.WriteLine("After setting to Rounding17: " + settings.SignificantDigitsType);

            // Lägg till några numeriska data för att demonstrera effekten
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(123.4567890123456789);
            worksheet.Cells["A2"].PutValue(9876543210.123456789);

            // Spara arbetsboken
            workbook.Save("SignificantDigitsTypeDemo.xlsx");
            Console.WriteLine("Workbook saved with SignificantDigitsType settings.");
        }
    }
}
```

### Se även

* enum [SignificantDigitsType](../../significantdigitstype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


