---
title: "Worksheet.RefreshPivotTables"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Aggiorna tutte le PivotTable in questo Worksheet"
type: docs
url: /it/net/aspose.cells/worksheet/refreshpivottables/
---
## RefreshPivotTables() {#refreshpivottables_1}

Aggiorna tutte le PivotTables in questo Worksheet.

```csharp
public void RefreshPivotTables()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRefreshPivotTablesDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine contenente pivot table
            Workbook workbook = new Workbook("example.xlsx");
            
            // Ottieni il primo foglio di lavoro che contiene pivot table
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiorna tutte le pivot table nel foglio di lavoro
            worksheet.RefreshPivotTables();
            
            // Salva la cartella di lavoro aggiornata
            workbook.Save("RefreshedPivotTables.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshPivotTables(PivotTableRefreshOption) {#refreshpivottables}

Aggiorna tutte le PivotTables in questo Worksheet.

```csharp
public bool RefreshPivotTables(PivotTableRefreshOption option)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzione | PivotTableRefreshOption | L'opzione per aggiornare la fonte dati della pivot table. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class WorksheetMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo
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
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;

            // Crea una tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            worksheet.RefreshPivotTables();

            int preCount = pivotTable.RowFields[0].PivotItems.Count;


            // Modifica i dati di origine
            worksheet.Cells["A2"].Value = "test2";
            worksheet.Cells["A3"].Value = "test3";

            // Crea opzioni di aggiornamento
            PivotTableRefreshOption options = new PivotTableRefreshOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All // Fixed: Changed ReserveAll to All
            };
            worksheet.RefreshPivotTables(options);
            int nowCount = pivotTable.RowFields[0].PivotItems.Count;
            Console.WriteLine(nowCount > preCount);
                        

            // Salva il risultato
            workbook.Save("WorksheetMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTableRefreshOption](../../../aspose.cells.pivot/pivottablerefreshoption/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


