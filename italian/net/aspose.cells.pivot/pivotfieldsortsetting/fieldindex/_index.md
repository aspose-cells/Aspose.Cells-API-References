---
title: "PivotFieldSortSetting.FieldIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotFieldSortSetting. Rappresenta l'indice del campo per cui è ordinato. 1 indica l'ordinamento del PivotField per le etichette, altri valori indicano l'ordinamento per il campo dati"
type: docs
url: /it/net/aspose.cells.pivot/pivotfieldsortsetting/fieldindex/
---
## PivotFieldSortSetting.FieldIndex property

Rappresenta l'indice del campo per cui è ordinato. -1 indica l'ordinamento del PivotField per le etichette, altri valori indicano l'ordinamento per il campo dati.

```csharp
[Obsolete("Use PivotFieldSortSetting.SortBy property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int FieldIndex { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotFieldSortSetting.SortBy. Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyFieldIndexDemo
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
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Ottieni l'impostazione di ordinamento del campo pivot
            PivotFieldSortSetting sortSetting = pivotTable.RowFields[0].SortSetting;

            // Visualizza il valore corrente di FieldIndex
            Console.WriteLine("Current FieldIndex value: " + sortSetting.FieldIndex);

            // Nota: FieldIndex è di sola lettura e PivotFieldSortSetting non può essere istanziato direttamente
            // poiché non ha un costruttore pubblico. Possiamo lavorare solo con l'istanza esistente
            // ottenuta dalla proprietà SortSetting del campo pivot.

            // Aggiorna la tabella pivot per applicare le modifiche
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Salva il risultato
            workbook.Save("PivotFieldSortSettingFieldIndexDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


