---
title: "CellsHelper.SignificantDigitsType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Eigenschaft. Ruft den Standardtyp signifikanter Stellen für die Ausgabe numerischer Werte ab und legt ihn fest. Standardwert ist G17"
type: docs
url: /de/net/aspose.cells/cellshelper/significantdigitstype/
---
## CellsHelper.SignificantDigitsType property

Liest und setzt den Standardtyp signifikanter Stellen für die Ausgabe numerischer Werte. Der Standardwert ist G17.

```csharp
public static SignificantDigitsType SignificantDigitsType { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperPropertySignificantDigitsTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Zeige den aktuellen SignificantDigitsType-Wert an
                Console.WriteLine("Current SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Setze einen neuen SignificantDigitsType-Wert
                CellsHelper.SignificantDigitsType = SignificantDigitsType.G17;
                Console.WriteLine("Updated SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Erstelle eine Arbeitsmappe, um den Effekt zu demonstrieren
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Füge einen numerischen Wert hinzu, der von signifikanten Stellen beeinflusst wird
                worksheet.Cells["A1"].PutValue(1.2345678912345678);
                worksheet.Cells["A2"].PutValue(1.2345678912345678);
                worksheet.Cells["A3"].Formula = "=A1+A2";

                // Berechne Formeln mit dem aktuellen Typ signifikanter Stellen
                workbook.CalculateFormula();

                // Ergebnis anzeigen
                Console.WriteLine("Calculation result: " + worksheet.Cells["A3"].Value);

                // Wechsle zu einem anderen Typ signifikanter Stellen
                CellsHelper.SignificantDigitsType = SignificantDigitsType.Rounding17;
                Console.WriteLine("Changed SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Berechne erneut mit dem neuen Typ signifikanter Stellen
                workbook.CalculateFormula();
                Console.WriteLine("Recalculated result: " + worksheet.Cells["A3"].Value);

                // Speichere die Arbeitsmappe
                workbook.Save("SignificantDigitsTypeDemo.xlsx");
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

* enum [SignificantDigitsType](../../significantdigitstype/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


