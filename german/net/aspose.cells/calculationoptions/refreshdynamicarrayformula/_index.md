---
title: "CalculationOptions.RefreshDynamicArrayFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CalculationOptions-Eigenschaft. Gibt an, ob dynamische Array-Formeln vor der Berechnung von Formeln aktualisiert werden sollen"
type: docs
url: /de/net/aspose.cells/calculationoptions/refreshdynamicarrayformula/
---
## CalculationOptions.RefreshDynamicArrayFormula property

Gibt an, ob dynamische Array‑Formeln vor der Berechnung von Formeln aktualisiert werden sollen.

```csharp
public bool RefreshDynamicArrayFormula { get; set; }
```

### Hinweise

Wenn diese Eigenschaft explizit angegeben wurde, wird der angegebene Wert verwendet, um zu bestimmen, ob dynamische Array‑Formeln aktualisiert werden sollen. Andernfalls ( [`UserSpecifiedRefreshDynamicArrayFormula`](../userspecifiedrefreshdynamicarrayformula/) ist falsch), hängt der Standardwert davon ab, welche Art von Formeln berechnet werden muss: Für die Berechnung von Formeln im Arbeitsbuch, wie z. B. [`CalculateFormula`](../../workbook/calculateformula/), wird diese Eigenschaft als true angenommen. In anderen Fällen, wie [`Calculate`](../../cell/calculate/) oder [`CalculateFormula`](../../worksheet/calculateformula/), wird diese Eigenschaft als false angenommen.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationOptionsPropertyRefreshDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine dynamische Array‑Formel hinzu, um die Funktionalität zu demonstrieren
            worksheet.Cells["A1"].Value = 1;
            worksheet.Cells["A2"].Value = 2;
            worksheet.Cells["A3"].Value = 3;
            worksheet.Cells["B1"].Formula = "=A1:A3"; // Dynamic array formula

            // CalculationOptions-Instanz erstellen
            CalculationOptions options = new CalculationOptions();

            try
            {
                // Standardwert von RefreshDynamicArrayFormula anzeigen
                Console.WriteLine("Default RefreshDynamicArrayFormula value: " + options.RefreshDynamicArrayFormula);

                // Setze die Eigenschaft auf true, um dynamische Array‑Formeln zu aktualisieren
                options.RefreshDynamicArrayFormula = true;
                Console.WriteLine("After setting to true: " + options.RefreshDynamicArrayFormula);

                // Formeln mit den angegebenen Optionen berechnen
                workbook.CalculateFormula(options);

                // Zeigen Sie das berechnete Ergebnis an
                Console.WriteLine("Dynamic array formula result: " + worksheet.Cells["B1"].Value);

                // Speichere die Arbeitsmappe
                workbook.Save("RefreshDynamicArrayFormulaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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


