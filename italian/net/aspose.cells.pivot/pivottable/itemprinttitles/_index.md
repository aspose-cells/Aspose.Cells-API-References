---
title: "PivotTable.ItemPrintTitles"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotTable property. Indica se i nomi PivotItem devono essere ripetuti in cima a ogni pagina stampata"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/itemprinttitles/
---
## PivotTable.ItemPrintTitles property

Indica se i nomi PivotItem devono essere ripetuti in cima a ogni pagina stampata.

```csharp
[Obsolete("Use PivotTable.RepeatItemsOnEachPrintedPage property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ItemPrintTitles { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotTable.RepeatItemsOnEachPrintedPage. Questo metodo sarà rimosso 12 mesi dopo, a partire da ottobre 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyItemPrintTitlesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Product C");
            worksheet.Cells["B4"].PutValue("East");
            worksheet.Cells["C4"].PutValue(3000);
            worksheet.Cells["A5"].PutValue("Product D");
            worksheet.Cells["B5"].PutValue("West");
            worksheet.Cells["C5"].PutValue(4000);

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Visualizza il valore corrente di ItemPrintTitles
            Console.WriteLine("Current ItemPrintTitles value: " + pivotTable.ItemPrintTitles);

            // Imposta ItemPrintTitles su true (questo è obsoleto, ma mostrato a scopo dimostrativo)
            pivotTable.ItemPrintTitles = true;

            // In alternativa, usa la proprietà non obsoleta
            pivotTable.RepeatItemsOnEachPrintedPage = true;

            // Aggiorna e calcola la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotTableItemPrintTitlesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


