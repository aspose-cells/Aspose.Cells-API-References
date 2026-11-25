---
title: "Class PivotFieldSortSetting"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Pivot.PivotFieldSortSetting class. Rappresenta l'impostazione per l'ordinamento dei campi pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotfieldsortsetting/
---
## PivotFieldSortSetting class

Rappresenta l'impostazione per l'ordinamento dei campi pivot.

```csharp
public class PivotFieldSortSetting
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Cell](../../aspose.cells.pivot/pivotfieldsortsetting/cell/) { get; } | Ordina per i valori nella riga o colonna. |
| [FieldIndex](../../aspose.cells.pivot/pivotfieldsortsetting/fieldindex/) { get; set; } | (**Obsolete.**) Rappresenta l'indice del campo per cui è ordinato. -1 indica l'ordinamento del PivotField per le etichette, altri valori indicano l'ordinamento per il campo dati. |
| [IsSimpleSort](../../aspose.cells.pivot/pivotfieldsortsetting/issimplesort/) { get; set; } | Indica se verrà applicata un'operazione di ordinamento dati semplice. |
| [IsSortByLabels](../../aspose.cells.pivot/pivotfieldsortsetting/issortbylabels/) { get; } | Indica se ordinare il campo per se stesso o per il campo dati. |
| [LineTypeSortedBy](../../aspose.cells.pivot/pivotfieldsortsetting/linetypesortedby/) { get; } | Il tipo di riga pivot ordinato per. |
| [SortBy](../../aspose.cells.pivot/pivotfieldsortsetting/sortby/) { get; set; } | Rappresenta l'indice del campo per cui è ordinato. Un valore di -1 indica l'ordinamento per i valori propri dell'elemento pivot. Quando è maggiore o uguale a zero, rappresenta l'indice del campo dati nella regione dei dati. |
| [SortType](../../aspose.cells.pivot/pivotfieldsortsetting/sorttype/) { get; set; } | Rappresenta il [`SortOrder`](../../aspose.cells/sortorder/). |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotFieldSortSettingDemo
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
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B2"].PutValue("East");
            worksheet.Cells["B3"].PutValue("West");
            worksheet.Cells["B4"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["C4"].PutValue(3000);

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Ottieni l'impostazione di ordinamento del campo pivot dalla tabella pivot
            // Nota: questo presuppone che la tabella pivot abbia impostazioni di ordinamento accessibili
            // Poiché non possiamo creare direttamente un nuovo PivotFieldSortSetting
            PivotFieldSortSetting sortSetting = pivotTable.RowFields[0].SortSetting;
            
            // Proprietà di visualizzazione (sola lettura)
            Console.WriteLine("SortType: " + sortSetting.SortType);
            Console.WriteLine("IsSortByLabels: " + sortSetting.IsSortByLabels);
            Console.WriteLine("FieldIndex: " + sortSetting.FieldIndex);
            Console.WriteLine("LineTypeSortedBy: " + sortSetting.LineTypeSortedBy);
            Console.WriteLine("IsSimpleSort: " + sortSetting.IsSimpleSort);
            Console.WriteLine("Cell: " + sortSetting.Cell);

            // Applica l'ordinamento alla tabella pivot (l'ordinamento reale verrebbe eseguito tramite i metodi della tabella pivot)
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Salva il risultato
            workbook.Save("PivotFieldSortSettingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


