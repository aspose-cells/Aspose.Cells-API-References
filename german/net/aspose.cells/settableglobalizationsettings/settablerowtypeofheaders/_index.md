---
title: "SettableGlobalizationSettings.SetTableRowTypeOfHeaders"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings-Methode. Legt den Typnamen der Tabellenzeilen fest, die den Tabellenkopf bilden."
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/settablerowtypeofheaders/
---
## SettableGlobalizationSettings.SetTableRowTypeOfHeaders method

Legt den Typnamen von Tabellenzeilen fest, die die Tabellenüberschrift enthalten.

```csharp
public void SetTableRowTypeOfHeaders(string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | der Typname von Tabellenzeilen |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfHeadersWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie eine Tabelle und fügen Sie einige Daten hinzu
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Header1");
            cells["B1"].PutValue("Header2");
            cells["A2"].PutValue("Value1");
            cells["B2"].PutValue("Value2");
            
            // Ein ListObject (Tabelle) erstellen
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // Erstellen Sie eine SettableGlobalizationSettings-Instanz
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Rufen Sie SetTableRowTypeOfHeaders mit benutzerdefiniertem Header-Typnamen auf
                settings.SetTableRowTypeOfHeaders("CustomHeaders");

                // Wenden Sie die Einstellungen auf die Arbeitsmappe an
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("Table header type name set to: CustomHeaders");
                Console.WriteLine("In formulas, '#CustomHeaders' will now represent the table header");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfHeaders method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("SetTableRowTypeOfHeadersDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


