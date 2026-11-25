---
title: "PivotFieldSortSetting.LineTypeSortedBy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotFieldSortSetting. Il tipo di linea pivot per cui è ordinato"
type: docs
url: /it/net/aspose.cells.pivot/pivotfieldsortsetting/linetypesortedby/
---
## PivotFieldSortSetting.LineTypeSortedBy property

Il tipo di riga pivot ordinato per.

```csharp
public PivotLineType LineTypeSortedBy { get; }
```

### Osservazioni

Funziona solo quando questo campo non è ordinato per etichette.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldSortSettingPropertyLineTypeSortedByDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 5;

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Ordina in ordine crescente con tipo di linea - fornisci una stringa vuota per il parametro cellName
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.GrandTotal, "");
            
            // Dimostra la proprietà LineTypeSortedBy
            Console.WriteLine("LineTypeSortedBy: " + pivotTable.RowFields[0].SortSetting.LineTypeSortedBy);
            
            // Modifica l'ordinamento per utilizzare il tipo di riga regolare
            pivotTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "C5");
            Console.WriteLine("LineTypeSortedBy after change: " + pivotTable.RowFields[0].SortSetting.LineTypeSortedBy);
        }
    }
}
```

### Vedi anche

* enum [PivotLineType](../../pivotlinetype/)
* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


