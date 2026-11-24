---
title: "GlobalizationSettings.GetDefaultSheetName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings-Methode. Gibt den Standardblattnamen für das automatische Hinzufügen eines Arbeitsblatts zurück. Standard ist Sheet"
type: docs
url: /de/net/aspose.cells/globalizationsettings/getdefaultsheetname/
---
## GlobalizationSettings.GetDefaultSheetName method

Gibt den Standardblattnamen für das automatische Hinzufügen eines Arbeitsblatts zurück. Standard ist "Sheet".

```csharp
public virtual string GetDefaultSheetName()
```

### Rückgabewert

der Standardblattname für das automatische Hinzufügen eines Arbeitsblatts

### Hinweise

Der automatisch hinzugefügte (z. B. durch [`Add`](../../worksheetcollection/add/)) Blattname wird der angegebene Name plus fortlaufende Nummer sein. Zum Beispiel möchte ein deutscher Benutzer möglicherweise den Blattnamen "Tabellenblatt2" anstelle von "Sheet2" haben. Dann kann der Benutzer diese Methode implementieren, um "Tabellenblatt" zurückzugeben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetDefaultSheetNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Benutzerdefinierte Globalisierungseinstellungen festlegen
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Den Standardblattnamen aus benutzerdefinierten Globalisierungseinstellungen abrufen
                string defaultSheetName = workbook.Settings.GlobalizationSettings.GetDefaultSheetName();
                Console.WriteLine($"Default sheet name retrieved: {defaultSheetName}");

                // Ein neues Arbeitsblatt hinzufügen, um die Namensgebung basierend auf dem benutzerdefinierten Standard zu demonstrieren
                int sheetIndex = workbook.Worksheets.Add();
                Worksheet newWorksheet = workbook.Worksheets[sheetIndex];
                Console.WriteLine($"New worksheet name after method call: {newWorksheet.Name}");

                Console.WriteLine("GetDefaultSheetName method demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDefaultSheetName method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("MethodGetDefaultSheetNameDemo.xlsx");
        }
    }

    // Implementierung benutzerdefinierter Globalisierungseinstellungen
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetDefaultSheetName()
        {
            return "CustomSheet"; // Custom default sheet name
        }
    }
}
```

### Siehe auch

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


