---
title: "PivotTable.ColumnGrand"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se il report PivotTable mostra i totali generali per le colonne"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/columngrand/
---
## PivotTable.ColumnGrand property

Indica se il report PivotTable mostra i totali generali per le colonne.

```csharp
[Obsolete("Use PivotTable.ShowColumnGrandTotals property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ColumnGrand { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare il metodo PivotTable.ShowColumnGrandTotals. Questo metodo sarà rimosso 12 mesi dopo, a partire da dicembre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyColumnGrandDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campo riga e campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Visualizza il valore corrente di ColumnGrand
            Console.WriteLine("Current ColumnGrand value: " + pivotTable.ColumnGrand);

            // Modifica la proprietà ColumnGrand
            pivotTable.ColumnGrand = false;

            // Calcola i dati per vedere l'effetto
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotTableColumnGrandDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


