---
title: "GlobalizationSettings.GetDefaultSheetName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metod. Hämtar standardnamnet för bladet när ett kalkylblad läggs till automatiskt. Standard är Sheet"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/getdefaultsheetname/
---
## GlobalizationSettings.GetDefaultSheetName method

Hämtar standardbladnamnet för att automatiskt lägga till ett kalkylblad. Standard är "Sheet".

```csharp
public virtual string GetDefaultSheetName()
```

### Returvärde

standardnamnet för bladet när ett kalkylblad läggs till automatiskt

### Anmärkningar

Det automatiskt tillagda (t.ex. via [`Add`](../../worksheetcollection/add/)) bladets namn kommer att vara det angivna namnet plus sekvensnummer. Till exempel kan en tysk användare vilja att bladnamnet blir "Tabellenblatt2" istället för "Sheet2". Då kan användaren implementera den här metoden för att returnera "Tabellenblatt".

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetDefaultSheetNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ställ in anpassade globaliseringsinställningar
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Hämta standardnamnet för bladet från anpassade globaliseringsinställningar
                string defaultSheetName = workbook.Settings.GlobalizationSettings.GetDefaultSheetName();
                Console.WriteLine($"Default sheet name retrieved: {defaultSheetName}");

                // Lägg till ett nytt kalkylblad för att demonstrera namngivning baserad på den anpassade standarden
                int sheetIndex = workbook.Worksheets.Add();
                Worksheet newWorksheet = workbook.Worksheets[sheetIndex];
                Console.WriteLine($"New worksheet name after method call: {newWorksheet.Name}");

                Console.WriteLine("GetDefaultSheetName method demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDefaultSheetName method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("MethodGetDefaultSheetNameDemo.xlsx");
        }
    }

    // Implementering av anpassade globaliseringsinställningar
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetDefaultSheetName()
        {
            return "CustomSheet"; // Custom default sheet name
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


