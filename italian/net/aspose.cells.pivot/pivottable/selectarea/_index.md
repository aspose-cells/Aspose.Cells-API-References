---
title: "PivotTable.SelectArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Seleziona un'area della visualizzazione della tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/selectarea/
---
## PivotTable.SelectArea method

Seleziona un'area della visualizzazione della tabella pivot.

```csharp
public PivotAreaCollection SelectArea(CellArea ca)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | CellArea | L'area della cella. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodSelectAreaWithCellAreaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Calcola i dati
            pivotTable.CalculateData();

            // Definisci l'area della cella da selezionare
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.StartColumn = 4;
            area.EndRow = 5;
            area.EndColumn = 6;

            try
            {
                // Chiama il metodo SelectArea con il parametro CellArea
                PivotAreaCollection selectedAreas = pivotTable.SelectArea(area);
                
                Console.WriteLine("SelectArea method executed successfully. Selected areas count: " + selectedAreas.Count);
                
                // Salva la cartella di lavoro per mostrare l'effetto
                workbook.Save("PivotTableSelectAreaDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SelectArea method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [PivotAreaCollection](../../pivotareacollection/)
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


