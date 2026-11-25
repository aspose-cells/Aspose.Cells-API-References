---
title: "PivotTable.TableRange2"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Restituisce un oggetto CellArea che rappresenta l'intervallo contenente l'intero report della PivotTable, inclusi i campi di pagina. Solo lettura"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/tablerange2/
---
## PivotTable.TableRange2 property

Restituisce un oggetto CellArea che rappresenta l'intervallo contenente l'intero report PivotTable, includendo i campi pagina. Sola lettura.

```csharp
public CellArea TableRange2 { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyTableRange2Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
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

            // Aggiungi una tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Calcola i dati
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Ottieni il TableRange2 che include l'intera tabella pivot
            CellArea tableRange2 = pivotTable.TableRange2;
            Console.WriteLine($"TableRange2: StartRow={tableRange2.StartRow}, StartColumn={tableRange2.StartColumn}, " +
                $"EndRow={tableRange2.EndRow}, EndColumn={tableRange2.EndColumn}");

            // Crea un intervallo basato su TableRange2
            Aspose.Cells.Range pivotRange = worksheet.Cells.CreateRange(
                tableRange2.StartRow, 
                tableRange2.StartColumn, 
                tableRange2.EndRow - tableRange2.StartRow + 1, 
                tableRange2.EndColumn - tableRange2.StartColumn + 1);

            // Restituisci l'indirizzo dell'intervallo
            Console.WriteLine($"Pivot Table Range: {pivotRange.Address}");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


