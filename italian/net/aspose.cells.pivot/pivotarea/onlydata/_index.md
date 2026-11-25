---
title: "PivotArea.OnlyData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotArea. Indica se sono selezionati solo i valori dei dati nell'area dati della visualizzazione per una selezione di elementi e non includono le etichette degli elementi"
type: docs
url: /it/net/aspose.cells.pivot/pivotarea/onlydata/
---
## PivotArea.OnlyData property

Indica se sono selezionati solo i valori dei dati (nell'area dati della visualizzazione) per una selezione di elementi e non includono le etichette degli elementi.

```csharp
public bool OnlyData { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyOnlyDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["A3"].PutValue("Clothing");
            worksheet.Cells["A4"].PutValue("Food");
            
            worksheet.Cells["B1"].PutValue("Revenue");
            worksheet.Cells["B2"].PutValue(5000);
            worksheet.Cells["B3"].PutValue(3000);
            worksheet.Cells["B4"].PutValue(2000);

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Configura l'area pivot
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.OnlyData = true; // Key property demonstration
            pivotArea.IsRowGrandIncluded = false;

            // Configurazione dell'output
            Console.WriteLine("OnlyData property is set to: " + pivotArea.OnlyData);
            
            workbook.Save("PivotAreaOnlyDataDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


