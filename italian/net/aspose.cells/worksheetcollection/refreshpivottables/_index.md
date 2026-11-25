---
title: "WorksheetCollection.RefreshPivotTables"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WorksheetCollection metodo. Aggiorna tutte le PivotTables nel file Excel"
type: docs
url: /it/net/aspose.cells/worksheetcollection/refreshpivottables/
---
## RefreshPivotTables() {#refreshpivottables_1}

Aggiorna tutte le PivotTables nel file Excel.

```csharp
public void RefreshPivotTables()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRefreshPivotTablesDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(3000);

            // Aggiungi tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 1);

            // Modifica i dati di origine
            worksheet.Cells["B2"].PutValue(1500);
            worksheet.Cells["B3"].PutValue(2500);

            // Aggiorna tutte le tabelle pivot nella cartella di lavoro
            workbook.Worksheets.RefreshPivotTables();

            // Salva la cartella di lavoro
            workbook.Save("RefreshPivotTablesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshPivotTables(PivotTableRefreshOption) {#refreshpivottables}

Aggiorna tutte le PivotTables nel file Excel.

```csharp
public bool RefreshPivotTables(PivotTableRefreshOption option)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzione | PivotTableRefreshOption | L'opzione per aggiornare l'origine dati delle tabelle pivot. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class WorksheetCollectionMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            cells["A1"].Value = "Category";
            cells["A2"].Value = "Fruit";
            cells["A3"].Value = "Vegetable";
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 1500;
            cells["B3"].Value = 2300;

            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B3", "E5", "SalesPivot");
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            PivotTableRefreshOption option = new PivotTableRefreshOption();

            workbook.Worksheets.RefreshPivotTables(option);

            Console.WriteLine(cells["F8"].StringValue);

            cells["B2"].Value = 2000;

            workbook.Worksheets.RefreshPivotTables(option);
            Console.WriteLine(cells["F8"].StringValue);
                       


            workbook.Save("WorksheetCollectionMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTableRefreshOption](../../../aspose.cells.pivot/pivottablerefreshoption/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


