---
title: "CalculationData.CellColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CalculationData‑Eigenschaft. Gibt den Spaltenindex der Zelle zurück, in der sich die Funktion befindet."
type: docs
url: /de/net/aspose.cells/calculationdata/cellcolumn/
---
## CalculationData.CellColumn property

Liest den Spaltenindex der Zelle, in der sich die Funktion befindet.

```csharp
public int CellColumn { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyCellColumnDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle ein neues Arbeitsbuch
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Beispieldaten mit Formeln in verschiedenen Spalten hinzufügen
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["B1"].PutValue(20);
                worksheet.Cells["C1"].Formula = "=SUM(A1:B1)";

                // Erstelle Berechnungsoptionen mit benutzerdefinierter Engine
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new CellColumnDemoEngine();

                // Formeln berechnen
                workbook.CalculateFormula(options);

                // Zeigen Sie das berechnete Ergebnis an
                Console.WriteLine("Calculated value in C1: " + worksheet.Cells["C1"].Value);

                // Ergebnis speichern
                workbook.Save("CellColumnDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CellColumnDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data != null)
            {
                // Greifen Sie auf die schreibgeschützte CellColumn‑Eigenschaft zu
                int columnIndex = data.CellColumn;
                Console.WriteLine($"Function is in column index: {columnIndex}");

                // Demonstrieren Sie die Verwendung der Spalteninformationen
                if (data.FunctionName == "SUM")
                {
                    double sum = 0;
                    for (int i = 0; i < data.ParamCount; i++)
                    {
                        object arg = data.GetParamValue(i);
                        if (arg is double)
                        {
                            sum += (double)arg;
                        }
                    }
                    data.CalculatedValue = sum;
                }
            }
        }
    }
}
```

### Siehe auch

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


