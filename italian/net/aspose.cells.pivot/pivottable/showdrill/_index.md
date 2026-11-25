---
title: "PivotTable.ShowDrill"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Ottiene e imposta se mostrare i pulsanti di espansione/collasso"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/showdrill/
---
## PivotTable.ShowDrill property

Ottiene e imposta se mostrare i pulsanti di espansione/collasso.

```csharp
public bool ShowDrill { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowDrillDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro e riempilo con dati di esempio
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Name = "Pivot";
            sheet.Cells["A1"].Value = "Category";
            sheet.Cells["B1"].Value = "Value";
            sheet.Cells["A2"].Value = "A";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["A3"].Value = "B";
            sheet.Cells["B3"].Value = 200;
            sheet.Cells["A4"].Value = "A";
            sheet.Cells["B4"].Value = 150;

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Configura la tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Abilita il drilldown e mostra gli indicatori di drill
            pivotTable.EnableDrilldown = true;
            pivotTable.ShowDrill = true;
            
            // Aggiorna e calcola i dati
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableShowDrillDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


