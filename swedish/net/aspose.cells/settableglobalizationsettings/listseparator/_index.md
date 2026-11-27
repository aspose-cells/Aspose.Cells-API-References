---
title: "SettableGlobalizationSettings.ListSeparator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings egenskap. Hämtar avgränsaren för listparametrar i funktion ...etc"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/listseparator/
---
## SettableGlobalizationSettings.ListSeparator property

Hämtar separatorn för lista, funktionsparametrar, ...etc.

```csharp
public override char ListSeparator { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyListSeparatorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en instans av SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Visa det aktuella ListSeparator‑värdet (standard är komma i de flesta språkversioner)
            Console.WriteLine("Current ListSeparator value: " + settings.ListSeparator);
            
            // Ställ in ett nytt ListSeparator‑värde (t.ex. semikolon)
            settings.SetListSeparator(';');
            
            // Applicera inställningarna på arbetsboken
            workbook.Settings.GlobalizationSettings = settings;
            
            // Demonstrera effekten av ListSeparator vid formeltolkning
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["A2"].PutValue("Data");
            
            // Skapa en formel som använder listavgränsaren
            worksheet.Cells["A3"].Formula = "=CONCATENATE(A1,A2)";
            
            // Formeln kommer att använda den anpassade listavgränsaren när den tolkas
            Console.WriteLine("Formula with custom separator: " + worksheet.Cells["A3"].Formula);
            
            // Spara arbetsboken
            workbook.Save("PropertyListSeparatorDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


