---
title: "PivotField.ShowValuesSetting"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Ottiene le impostazioni di visualizzazione dei valori quando è in uso il calcolo ShowDataAs"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/showvaluessetting/
---
## PivotField.ShowValuesSetting property

Ottiene le impostazioni per mostrare i valori quando è in uso il calcolo ShowDataAs.

```csharp
public PivotShowValuesSetting ShowValuesSetting { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowValuesSettingDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 3000;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 1500;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 2500;
            cells["A7"].Value = "Banana";
            cells["B7"].Value = 3500;

            // Crea tabella pivot
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B7", "C10", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Aggiungi campi di riga e di dati
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[0];
            
            // Configura ShowValuesSetting per visualizzare come percentuale del totale
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
            
            // Calcola e aggiorna la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFieldShowValuesSettingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotShowValuesSetting](../../pivotshowvaluessetting/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


