---
title: "CalculationOptions.UserSpecifiedRefreshDynamicArrayFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CalculationOptions-Eigenschaft. Gibt an, ob der Benutzer das Verhalten zum Aktualisieren dynamischer Array-Formeln vor der Berechnung bestimmter Formeln explizit festgelegt hat."
type: docs
url: /de/net/aspose.cells/calculationoptions/userspecifiedrefreshdynamicarrayformula/
---
## CalculationOptions.UserSpecifiedRefreshDynamicArrayFormula property

Gibt an, ob der Benutzer das Verhalten zum Aktualisieren dynamischer Array‑Formeln vor der Berechnung bestimmter Formeln explizit festgelegt hat.

```csharp
public bool UserSpecifiedRefreshDynamicArrayFormula { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationOptionsPropertyUserSpecifiedRefreshDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Erstelle ein Beispiel-Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten hinzu, um das Beispiel sinnvoll zu machen.
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // CalculationOptions-Instanz erstellen
                CalculationOptions options = new CalculationOptions();

                // Den aktuellen Wert der UserSpecifiedRefreshDynamicArrayFormula-Eigenschaft anzeigen
                Console.WriteLine("UserSpecifiedRefreshDynamicArrayFormula value: " +
                    options.UserSpecifiedRefreshDynamicArrayFormula);

                // Zeigen, wie die Eigenschaft das Verhalten beeinflusst
                Console.WriteLine("UserSpecifiedRefreshDynamicArrayFormula has been demonstrated");

                // Ergebnis speichern
                workbook.Save("UserSpecifiedRefreshDynamicArrayFormulaDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


