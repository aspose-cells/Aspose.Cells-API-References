---
title: "PivotField.GetFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Methode. Gibt die Formel des berechneten Feldes zurück. Funktioniert nur für das berechnete Feld."
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/getformula/
---
## PivotField.GetFormula method

Liest die Formel des berechneten Feldes. Funktioniert nur für das berechnete Feld.

```csharp
public string GetFormula()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGetFormulaDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Bike";
            worksheet.Cells["B4"].Value = 1500;
            
            // Pivot-Tabelle erstellen
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Berechnetes Feld mit Formel hinzufügen
            pivotTable.AddCalculatedField("=ABS('Sales')", "Absolute Sales");
            
            // Formel aus dem berechneten Feld abrufen
            PivotFieldCollection fields = pivotTable.DataFields;
            string formula = fields[fields.Count - 1].GetFormula();
            
            // Formel ausgeben
            Console.WriteLine("Calculated field formula: " + formula);
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


