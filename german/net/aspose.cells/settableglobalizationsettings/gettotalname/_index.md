---
title: "SettableGlobalizationSettings.GetTotalName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings-Methode. Gibt den Gesamtnamen einer bestimmten Funktion zurück."
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/gettotalname/
---
## SettableGlobalizationSettings.GetTotalName method

Gibt den Gesamtnamen einer bestimmten Funktion zurück.

```csharp
public override string GetTotalName(ConsolidationFunction functionType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| functionType | ConsolidationFunction | Der Funktionstyp. |

### Rückgabewert

Der Gesamtnamen der Funktion.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Instanz von SettableGlobalizationSettings
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // Rufen Sie GetTotalName mit ConsolidationFunction.Sum auf.
                string totalName = globalizationSettings.GetTotalName(ConsolidationFunction.Sum);
                
                // Ergebnis anzeigen
                Console.WriteLine($"Total name for Sum function: {totalName}");

                // Fügen Sie Daten hinzu, um die Wirkung zu demonstrieren (obwohl GetTotalName das Tabellenblatt nicht verändert).
                worksheet.Cells["A1"].PutValue("Values");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["B1"].PutValue("Total");
                worksheet.Cells["B4"].Formula = "=SUM(A2:A4)";
                
                // Formeln berechnen
                workbook.CalculateFormula();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTotalName method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("SettableGlobalizationSettingsMethodGetTotalNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


