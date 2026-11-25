---
title: "PivotTable.MoveTo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Sposta la PivotTable in una posizione diversa nel foglio di lavoro"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/moveto/
---
## MoveTo(int, int) {#moveto}

Sposta la PivotTable in una posizione diversa nel foglio di lavoro.

```csharp
public void MoveTo(int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | indice della riga. |
| colonna | Int32 | indice colonna. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodMoveToWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(1500);
            worksheet.Cells["B3"].PutValue(2500);

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");

            // Calcola i dati per popolare la tabella pivot
            pivotTable.CalculateData();

            try
            {
                // Chiama il metodo MoveTo con parametri (Int32, Int32) per spostare la tabella pivot
                pivotTable.MoveTo(5, 2); // Move to row 5, column 2
                
                Console.WriteLine("Pivot table moved successfully to new location (5,2)");
                
                // Ricalcola i dati per aggiornare la tabella pivot spostata
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing MoveTo method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("PivotTableMethodMoveToWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## MoveTo(int, int, int) {#moveto_1}

Sposta la PivotTable in una posizione diversa nel foglio di lavoro.

```csharp
public void MoveTo(int sheetIndex, int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | Int32 | l'indice del foglio di lavoro di destinazione |
| riga | Int32 | indice della riga. |
| colonna | Int32 | indice colonna. |

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## MoveTo(string) {#moveto_2}

Sposta la PivotTable in una posizione diversa nel foglio di lavoro.

```csharp
public void MoveTo(string destCellName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destCellName | String | il nome della cella di destinazione. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodMoveToWithStringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Imposta dati di esempio
            cells["A1"].Value = "fruit";
            cells["A2"].Value = "grape";
            cells["A3"].Value = "blueberry";
            cells["A4"].Value = "kiwi";
            cells["A5"].Value = "cherry";
            cells["A6"].Value = "grape";
            cells["A7"].Value = "blueberry";
            cells["A8"].Value = "kiwi";
            cells["A9"].Value = "cherry";

            cells["B1"].Value = "year";
            cells["B2"].Value = 2020;
            cells["B3"].Value = 2020;
            cells["B4"].Value = 2020;
            cells["B5"].Value = 2020;
            cells["B6"].Value = 2021;
            cells["B7"].Value = 2021;
            cells["B8"].Value = 2021;
            cells["B9"].Value = 2021;

            cells["C1"].Value = "amount";
            cells["C2"].Value = 50;
            cells["C3"].Value = 60;
            cells["C4"].Value = 70;
            cells["C5"].Value = 80;
            cells["C6"].Value = 90;
            cells["C7"].Value = 100;
            cells["C8"].Value = 110;
            cells["C9"].Value = 120;

            // Crea tabella pivot
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            
            // Aggiungi campi alla tabella pivot
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Imposta lo stile e aggiorna
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            sheet.RefreshPivotTables();

            // Sposta la tabella pivot in una nuova posizione
            pivot.MoveTo("H16");
            sheet.RefreshPivotTables();

            // Salva la cartella di lavoro
            book.Save("PivotTableMoveToExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


