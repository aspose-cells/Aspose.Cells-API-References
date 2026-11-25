---
title: "PivotTable.PageFieldOrder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Ottiene e imposta l'ordine in cui i campi di pagina vengono aggiunti al layout dei report della PivotTable"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/pagefieldorder/
---
## PivotTable.PageFieldOrder property

Restituisce e imposta l'ordine in cui i campi pagina vengono aggiunti al layout del report PivotTable.

```csharp
public PrintOrderType PageFieldOrder { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPageFieldOrderDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            var cells = worksheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["C1"].Value = "Region";
            cells["D1"].Value = "Sales";
            
            // Aggiungi righe di dati di esempio
            for (int i = 2; i <= 10; i++)
            {
                cells[$"A{i}"].Value = $"Category{(i % 3) + 1}";
                cells[$"B{i}"].Value = $"Product{(i % 4) + 1}";
                cells[$"C{i}"].Value = $"Region{(i % 2) + 1}";
                cells[$"D{i}"].Value = i * 100;
            }

            // Crea tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:D11", "F5", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Aggiungi campi alle aree
            pivotTable.AddFieldToArea(PivotFieldType.Page, pivotTable.BaseFields["Category"]);
            pivotTable.AddFieldToArea(PivotFieldType.Page, pivotTable.BaseFields["Region"]);
            pivotTable.AddFieldToArea(PivotFieldType.Row, pivotTable.BaseFields["Product"]);
            pivotTable.AddFieldToArea(PivotFieldType.Data, pivotTable.BaseFields["Sales"]);

            // Imposta l'ordine dei campi di pagina e il conteggio di avvolgimento
            pivotTable.PageFieldOrder = PrintOrderType.DownThenOver;
            pivotTable.PageFieldWrapCount = 2;

            // Salva la cartella di lavoro
            workbook.Save("PivotTablePageFieldOrderDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PrintOrderType](../../../aspose.cells/printordertype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


