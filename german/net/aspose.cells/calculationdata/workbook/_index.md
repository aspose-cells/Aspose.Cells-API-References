---
title: "CalculationData.Workbook"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CalculationData-Eigenschaft. Gibt das Workbook-Objekt zurück, in dem die Funktion ist"
type: docs
url: /de/net/aspose.cells/calculationdata/workbook/
---
## CalculationData.Workbook property

Liest das Workbook-Objekt, in dem sich die Funktion befindet.

```csharp
public Workbook Workbook { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyWorkbookDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten und Formel hinzufügen
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].Formula = "=CUSTOMFUNC()";

            // Erstelle Berechnungsoptionen und registriere eine benutzerdefinierte Berechnungs-Engine
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomCalcEngine();

            // Löse die Berechnung mit Optionen aus, um die Verwendung der Workbook-Eigenschaft zu demonstrieren
            workbook.CalculateFormula(options);

            // Zeige das Ergebnis der Berechnung an
            Console.WriteLine("Calculated value in B1: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("Modified value in C1: " + worksheet.Cells["C1"].Value);

            // Ergebnis speichern
            workbook.Save("PropertyWorkbookDemo.xlsx");
        }

        private class CustomCalcEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName == "CUSTOMFUNC")
                {
                    // Greife auf die Workbook-Eigenschaft von CalculationData zu
                    Workbook currentWorkbook = data.Workbook;
                    Worksheet currentSheet = currentWorkbook.Worksheets[0];

                    // Demonstriere die Verwendung von Workbook zum Manipulieren von Daten
                    double inputValue = (double)currentSheet.Cells["A1"].Value;
                    currentSheet.Cells["C1"].PutValue(inputValue * 2);

                    // Setze das berechnete Ergebnis
                    data.CalculatedValue = inputValue * 3;
                }
            }
        }
    }
}
```

### Siehe auch

* class [Workbook](../../workbook/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


