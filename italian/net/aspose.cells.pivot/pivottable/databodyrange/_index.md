---
title: "PivotTable.DataBodyRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Restituisce un oggetto CellArea che rappresenta l'intervallo che contiene l'area dati nell'elenco tra la riga di intestazione e la riga di inserimento. Sola lettura"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/databodyrange/
---
## PivotTable.DataBodyRange property

Restituisce un oggetto [`CellArea`](../../../aspose.cells/cellarea/) che rappresenta l'intervallo che contiene l'area dati nell'elenco tra la riga di intestazione e la riga di inserimento. Sola lettura.

```csharp
public CellArea DataBodyRange { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataBodyRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Aggiungi dati di esempio per la tabella pivot
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bike";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Car";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bike";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Car";
            cells["B5"].Value = 2500;

            // Aggiungi tabella pivot
            int pivotIndex = sheet.PivotTables.Add("A7", "A1:B5", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            // Configura la tabella pivot
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Aggiorna i dati della tabella pivot
            pivot.RefreshData();
            pivot.CalculateData();

            // Dimostra l'uso di DataBodyRange
            CellArea dataBodyArea = pivot.DataBodyRange;
            Console.WriteLine($"Data body range: StartRow={dataBodyArea.StartRow}, EndRow={dataBodyArea.EndRow}, StartColumn={dataBodyArea.StartColumn}, EndColumn={dataBodyArea.EndColumn}");

            // Salva la cartella di lavoro
            workbook.Save("PivotTableDataBodyRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


