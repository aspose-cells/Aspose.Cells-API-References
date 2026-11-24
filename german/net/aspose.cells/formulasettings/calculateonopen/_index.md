---
title: "FormulaSettings.CalculateOnOpen"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormulaSettings-Eigenschaft. Gibt an, ob die Anwendung beim Öffnen der Arbeitsmappe eine vollständige Berechnung durchführen muss."
type: docs
url: /de/net/aspose.cells/formulasettings/calculateonopen/
---
## FormulaSettings.CalculateOnOpen property

Gibt an, ob die Anwendung beim Öffnen der Arbeitsmappe eine vollständige Berechnung durchführen muss.

```csharp
public bool CalculateOnOpen { get; set; }
```

### Hinweise

Diese Eigenschaft dient ausschließlich dem Speichern der Einstellungen in die resultierende Tabellendatei, damit andere Anwendungen (wie MS Excel) beim Laden der Datei entsprechend reagieren können. Aus Leistungsgründen für die meisten Benutzeranwendungen berechnen wir keine Formel in der Arbeitsmappe automatisch, unabhängig davon, welcher Wert für diese Eigenschaft festgelegt wurde.

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculateOnOpenDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Formel in Zelle A1 festlegen, die sich auf B1 bezieht
            worksheet.Cells["A1"].Formula = "=B1";
            
            // Wert in Zelle B1 festlegen
            worksheet.Cells["B1"].PutValue(10);
            
            // Automatische Formelberechnung beim Öffnen deaktivieren
            workbook.Settings.FormulaSettings.CalculateOnOpen = false;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            // Gespeicherte Arbeitsmappe erneut öffnen
            Workbook reopenedWorkbook = new Workbook("output.xlsx");
            
            // Überprüfen, dass die Formel beim Öffnen nicht berechnet wurde
            Console.WriteLine("A1 value (should be 0 before calculation): " + reopenedWorkbook.Worksheets[0].Cells["A1"].IntValue);
            
            // Formeln manuell berechnen
            reopenedWorkbook.CalculateFormula();
            
            // Überprüfen, dass die Formel berechnet wurde
            Console.WriteLine("A1 value (should be 10 after calculation): " + reopenedWorkbook.Worksheets[0].Cells["A1"].IntValue);
        }
    }
}
```

### Siehe auch

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


