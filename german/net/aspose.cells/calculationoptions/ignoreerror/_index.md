---
title: "CalculationOptions.IgnoreError"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CalculationOptions-Eigenschaft. Gibt an, ob Fehler, die bei der Berechnung von Formeln auftreten, ignoriert werden sollen. Der Fehler kann eine nicht unterstützte Funktion, externe Links usw. sein. Der Standardwert ist true"
type: docs
url: /de/net/aspose.cells/calculationoptions/ignoreerror/
---
## CalculationOptions.IgnoreError property

Gibt an, ob beim Berechnen von Formeln auftretende Fehler ignoriert werden sollen. Der Fehler kann eine nicht unterstützte Funktion, externe Verknüpfungen usw. sein. Der Standardwert ist true.

```csharp
public bool IgnoreError { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyIgnoreErrorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einen benannten Bereich hinzu, der nicht existiert, um die Fehlerbehandlung zu demonstrieren
            worksheet.Cells["A1"].Formula = "=NONEXISTENTNAME()";
            
            // Berechnen mit IgnoreError = false (wirft einen Fehler)
            try
            {
                workbook.CalculateFormula(new CalculationOptions() { IgnoreError = false });
                Console.WriteLine("Calculation completed without ignoring errors");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error occurred (expected): " + ex.Message);
            }

            // Berechnen mit IgnoreError = true (unterdrückt den Fehler)
            try
            {
                workbook.CalculateFormula(new CalculationOptions() { IgnoreError = true });
                Console.WriteLine("Calculation completed while ignoring errors");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error occurred (unexpected): " + ex.Message);
            }
        }
    }
}
```

### Siehe auch

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


