---
title: "SettablePivotGlobalizationSettings.GetTextOfProtectedName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettablePivotGlobalizationSettings-Methode. Gibt den Text für den angegebenen geschützten Namen zurück"
type: docs
url: /de/net/aspose.cells/settablepivotglobalizationsettings/gettextofprotectedname/
---
## SettablePivotGlobalizationSettings.GetTextOfProtectedName method

Ermittelt den Text für den angegebenen geschützten Namen.

```csharp
public override string GetTextOfProtectedName(string protectedName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| protectedName | String | Der geschützte Name in der PivotTable. |

### Rückgabewert

Die lokalen geschützten Namen der PivotTable.

### Hinweise

In Ms Excel dürfen einige Namen nicht als Name von PivotFields in einer PivotTable verwendet werden. Sie unterscheiden sich je nach Region; der Benutzer kann sie je nach verwendeter Region explizit angeben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfProtectedNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Beispieldaten zum Kontext hinzufügen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Erstelle eine Instanz von SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Legen Sie einen benutzerdefinierten Text für einen geschützten Namen fest
                settings.SetTextOfProtectedName("Sum", "Total Sum");

                // Rufen Sie den Text des geschützten Namens ab
                string protectedNameText = settings.GetTextOfProtectedName("Sum");

                Console.WriteLine($"Text for protected name 'Sum': {protectedNameText}");

                // Speichere die Arbeitsmappe
                workbook.Save("GetTextOfProtectedNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfProtectedName: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


