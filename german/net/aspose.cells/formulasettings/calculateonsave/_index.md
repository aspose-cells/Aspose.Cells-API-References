---
title: "FormulaSettings.CalculateOnSave"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormulaSettings-Eigenschaft. Gibt an, ob die Arbeitsmappe vor dem Speichern des Dokuments im manuellen Berechnungsmodus neu berechnet werden soll."
type: docs
url: /de/net/aspose.cells/formulasettings/calculateonsave/
---
## FormulaSettings.CalculateOnSave property

Gibt an, ob die Arbeitsmappe im manuellen Berechnungsmodus vor dem Speichern des Dokuments neu berechnet werden soll.

```csharp
public bool CalculateOnSave { get; set; }
```

### Hinweise

Diese Eigenschaft dient ausschließlich dem Speichern der Einstellungen in die resultierende Tabellendatei, damit andere Anwendungen (wie MS Excel) beim Laden und Bearbeiten der Datei entsprechend reagieren können. Aus Leistungsgründen für die meisten Benutzeranwendungen berechnen wir keine Formeln in der Arbeitsmappe automatisch, unabhängig davon, welcher Wert für diese Eigenschaft festgelegt wurde.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculateOnSaveDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf das Arbeitsblatt zu und fügen Sie einige Daten hinzu.
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // CalculateOnSave deaktivieren (Standard ist false).
            workbook.Settings.FormulaSettings.CalculateOnSave = false;
            
            // Speichern ohne Formeln zu berechnen.
            workbook.Save("output_without_calculation.xlsx");

            // CalculateOnSave aktivieren.
            workbook.Settings.FormulaSettings.CalculateOnSave = true;
            
            // Speichern mit Formelberechnung.
            workbook.Save("output_with_calculation.xlsx");
        }
    }
}
```

### Siehe auch

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


