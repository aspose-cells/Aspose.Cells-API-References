---
title: "PivotField.GetFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotField. Ottiene la formula del campo calcolato. Funziona solo per il campo calcolato"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/getformula/
---
## PivotField.GetFormula method

Recupera la formula del campo calcolato. Funziona solo per il campo calcolato.

```csharp
public string GetFormula()
```

### Esempi

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
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Bike";
            worksheet.Cells["B4"].Value = 1500;
            
            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Aggiungi un campo calcolato con formula
            pivotTable.AddCalculatedField("=ABS('Sales')", "Absolute Sales");
            
            // Ottieni la formula dal campo calcolato
            PivotFieldCollection fields = pivotTable.DataFields;
            string formula = fields[fields.Count - 1].GetFormula();
            
            // Visualizza la formula
            Console.WriteLine("Calculated field formula: " + formula);
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


