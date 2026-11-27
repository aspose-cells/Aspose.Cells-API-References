---
title: "WorkbookSettings.LanguageCode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings egenskap. Hämtar eller anger användargränssnittsspråket för Workbook-versionen baserat på CountryCode som har sparat filen"
type: docs
url: /sv/net/aspose.cells/workbooksettings/languagecode/
---
## WorkbookSettings.LanguageCode property

Hämtar eller anger användargränssnittsspråket för arbetsbokens version baserat på landskoden som har sparat filen.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till arbetsboksinställningar
            WorkbookSettings settings = workbook.Settings;

            // Ställ in språkkod till tyska (Tyskland)
            settings.LanguageCode = CountryCode.Germany;

            // Visa den aktuella språkkoden
            Console.WriteLine("Current Language Code: " + settings.LanguageCode);

            // Ändra språkkod till franska (Frankrike)
            settings.LanguageCode = CountryCode.France;
            Console.WriteLine("Updated Language Code: " + settings.LanguageCode);

            // Spara arbetsboken
            workbook.Save("WorkbookSettings_LanguageCodeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [CountryCode](../../countrycode/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


