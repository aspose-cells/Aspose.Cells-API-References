---
title: "PivotArea.PivotArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore di PivotArea. Presenta l'area selezionata della PivotTable"
type: docs
url: /it/net/aspose.cells.pivot/pivotarea/pivotarea/
---
## PivotArea constructor

Presenta l'area selezionata della PivotTable.

```csharp
public PivotArea(PivotTable table)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tabella | PivotTable |  |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaMethodctorWithPivotTableDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Dimostra il costruttore di PivotArea con parametro PivotTable
            PivotArea pivotArea = new PivotArea(pivotTable);
            
            // Configura l'area pivot
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.RuleType = PivotAreaType.Normal;
            
            // Salva la cartella di lavoro
            workbook.Save("PivotAreaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../../pivottable/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


