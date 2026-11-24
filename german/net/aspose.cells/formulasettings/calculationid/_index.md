---
title: "FormulaSettings.CalculationId"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormulaSettings-Eigenschaft. Gibt die Version der Berechnungs-Engine an, die zum Berechnen von Werten in der Arbeitsmappe verwendet wird."
type: docs
url: /de/net/aspose.cells/formulasettings/calculationid/
---
## FormulaSettings.CalculationId property

Gibt die Version der Berechnungs-Engine an, die zum Berechnen von Werten in der Arbeitsmappe verwendet wird.

```csharp
public string CalculationId { get; set; }
```

### Hinweise

Diese Eigenschaft dient ausschließlich dem Speichern der Einstellungen in die resultierende Tabellendatei, damit andere Anwendungen (wie MS Excel) beim Laden und Verarbeiten der Datei entsprechend reagieren können. Im Fall von MS Excel wird, wenn der Wert dieser Eigenschaft kleiner ist als die Kennung der Neuberechnungs-Engine, die mit der Anwendung verbunden ist, die die Datei öffnet, die Anwendung die Ergebnisse aller Formeln in dieser Arbeitsmappe sofort nach dem Laden der Datei neu berechnen. Aus Leistungsgründen für die meisten Benutzeranwendungen berechnen wir keine Formel in der Arbeitsmappe automatisch, unabhängig davon, welcher Wert für diese Eigenschaft festgelegt wurde.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculationIdDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Formel festlegen, die sich basierend auf CalculationId unterschiedlich verhält
            Cell cell = sheet.Cells["A1"];
            cell.Formula = "=AND(\"a\",true)";
            
            // Berechnen ohne CalculationId (Standardverhalten)
            wb.CalculateFormula();
            Console.WriteLine("Without CalculationId: " + cell.Value);
            
            // CalculationId festlegen und neu berechnen
            wb.Settings.FormulaSettings.CalculationId = "181029";
            wb.CalculateFormula();
            Console.WriteLine("With CalculationId 181029: " + cell.BoolValue);
        }
    }
}
```

### Siehe auch

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


