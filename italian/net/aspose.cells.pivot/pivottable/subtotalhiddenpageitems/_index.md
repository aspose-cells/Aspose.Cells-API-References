---
title: "PivotTable.SubtotalHiddenPageItems"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se gli elementi dei campi pagina nascosti nel report PivotTable sono inclusi nei subtotali di righe e colonne, nei totali dei blocchi e nei totali generali. Il valore predefinito è False"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/subtotalhiddenpageitems/
---
## PivotTable.SubtotalHiddenPageItems property

Indica se gli elementi dei campi pagina nascosti nel report PivotTable sono inclusi nei subtotali di riga e colonna, nei totali di blocco e nei totali complessivi. Il valore predefinito è False.

```csharp
public bool SubtotalHiddenPageItems { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertySubtotalHiddenPageItemsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Apple";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Orange";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            
            cells["A4"].Value = "Banana";
            cells["B4"].Value = "North";
            cells["C4"].Value = 1500;
            
            cells["A5"].Value = "Apple";
            cells["B5"].Value = "South";
            cells["C5"].Value = 1200;

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Aggiungi campi
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Imposta la proprietà SubtotalHiddenPageItems
            pivotTable.SubtotalHiddenPageItems = true;
            Console.WriteLine("SubtotalHiddenPageItems set to: " + pivotTable.SubtotalHiddenPageItems);

            // Aggiorna e calcola i dati
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotTable_SubtotalHiddenPageItemsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


