---
title: "PivotTable.ShowEmptyRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se includere righe vuote nella tabella"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/showemptyrow/
---
## PivotTable.ShowEmptyRow property

Indica se includere righe vuote nella tabella.

```csharp
public bool ShowEmptyRow { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyShowEmptyRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio con alcune righe vuote
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Product";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["B2"].Value = "TV";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Electronics";
            worksheet.Cells["B3"].Value = "";
            worksheet.Cells["C3"].Value = "";
            
            worksheet.Cells["A4"].Value = "Furniture";
            worksheet.Cells["B4"].Value = "Chair";
            worksheet.Cells["C4"].Value = 500;
            
            worksheet.Cells["A5"].Value = "Furniture";
            worksheet.Cells["B5"].Value = "";
            worksheet.Cells["C5"].Value = "";

            // Crea una tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Visualizza il valore corrente di ShowEmptyRow
            Console.WriteLine("Initial ShowEmptyRow value: " + pivotTable.ShowEmptyRow);

            // Mostra righe vuote nella tabella pivot
            pivotTable.ShowEmptyRow = true;
            Console.WriteLine("ShowEmptyRow set to: " + pivotTable.ShowEmptyRow);

            // Calcola i dati per popolare la tabella pivot
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotTableShowEmptyRowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


