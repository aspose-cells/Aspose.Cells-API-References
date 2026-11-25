---
title: "PivotTable.GrandTotalName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotTable property. Restituisce l'etichetta visualizzata nell'intestazione della colonna o della riga del totale generale. Il valore predefinito è la stringa Grand Total"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/grandtotalname/
---
## PivotTable.GrandTotalName property

Restituisce l'etichetta visualizzata nell'intestazione della colonna o della riga del totale generale. Il valore predefinito è la stringa "Grand Total".

```csharp
public string GrandTotalName { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyGrandTotalNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Laptop";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Laptop";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 1500;
            
            worksheet.Cells["A4"].Value = "Phone";
            worksheet.Cells["B4"].Value = "North";
            worksheet.Cells["C4"].Value = 800;
            
            worksheet.Cells["A5"].Value = "Phone";
            worksheet.Cells["B5"].Value = "South";
            worksheet.Cells["C5"].Value = 1200;

            // Crea una tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Aggiungi campi di riga e di dati
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Visualizza il valore corrente di GrandTotalName
            Console.WriteLine("Current GrandTotalName: " + pivotTable.GrandTotalName);

            // Modifica il GrandTotalName
            pivotTable.GrandTotalName = "Total Summary";

            // Calcola i dati e aggiorna la tabella pivot
            pivotTable.CalculateData();
            pivotTable.RefreshData();

            // Salva la cartella di lavoro
            workbook.Save("PivotTableGrandTotalNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


