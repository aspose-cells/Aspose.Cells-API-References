---
title: "PivotTableRefreshOption.PivotTableRefreshOption"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore PivotTableRefreshOption. Rappresenta le opzioni di aggiornamento dell'origine dati della tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottablerefreshoption/pivottablerefreshoption/
---
## PivotTableRefreshOption constructor

Rappresenta le opzioni di aggiornamento dell'origine dati della tabella pivot.

```csharp
public PivotTableRefreshOption()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableRefreshOptionMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            var cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Apple";
            cells["B2"].Value = "North";            cells["C2"].Value = 1000;
            cells["A3"].Value = "Orange";            cells["B3"].Value = "South";            cells["C3"].Value = 2000;
            cells["A4"].Value = "Banana";            cells["B4"].Value = "East";            cells["C4"].Value = 3000;
            cells["A5"].Value = "Apple";            cells["B5"].Value = "South";            cells["C5"].Value = 4000;
            
            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Crea e configura le opzioni di aggiornamento utilizzando il costruttore
            PivotTableRefreshOption refreshOption = new PivotTableRefreshOption();
            refreshOption.ReserveMissingPivotItemType = ReserveMissingPivotItemType.None;
            
            // Aggiorna la tabella pivot con le opzioni
            pivotTable.RefreshData(refreshOption);
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableRefreshDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [PivotTableRefreshOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


