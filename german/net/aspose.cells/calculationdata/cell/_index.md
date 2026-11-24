---
title: "CalculationData.Cell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CalculationData-Eigenschaft. Gibt das Cell-Objekt zurück, in dem die Funktion ist"
type: docs
url: /de/net/aspose.cells/calculationdata/cell/
---
## CalculationData.Cell property

Liest das Cell-Objekt, in dem sich die Funktion befindet.

```csharp
public Cell Cell { get; }
```

### Hinweise

Wenn eine Formel berechnet wird, ohne sie in einer Zelle zu setzen, zum Beispiel mit [`CalculateFormula`](../../worksheet/calculateformula/), wird die Formel so berechnet, als wäre sie in Zelle A1 gesetzt, sodass sowohl [`CellRow`](../cellrow/) als auch [`CellColumn`](../cellcolumn/) 0 sind. Allerdings wurde die Zelle A1 im Arbeitsblatt möglicherweise noch nicht instanziiert. Für solche Situationen ist diese Eigenschaft daher null.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyCellDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle ein neues Arbeitsbuch
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Füge einige Daten hinzu, um das Beispiel sinnvoll zu machen.
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

                // Erstelle Berechnungsoptionen mit benutzerdefinierter Engine
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new CellDemoEngine();

                // Formeln mit Optionen berechnen
                workbook.CalculateFormula(options);

                // Ergebnis anzeigen
                Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);

                // Ergebnis speichern
                workbook.Save("CellDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CellDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                // Greife auf die schreibgeschützte Cell-Eigenschaft zu
                Cell cell = data.Cell;
                Console.WriteLine($"Function is in cell: {cell.Name}");
                Console.WriteLine($"Cell value: {cell.StringValue}");
                Console.WriteLine($"Cell row: {cell.Row}, column: {cell.Column}");

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
```

### Siehe auch

* class [Cell](../../cell/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


