---
title: "Enum PivotLineType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Pivot.PivotLineType. Specifica il tipo di PivotLine"
type: docs
url: /it/net/aspose.cells.pivot/pivotlinetype/
---
## PivotLineType enumeration

Specifica il tipo di PivotLine.

```csharp
public enum PivotLineType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Regular | `0` | PivotLine regolare con elementi pivot. |
| Subtotal | `1` | Riga di subtotale. |
| GrandTotal | `2` | Riga Totale Generale. |
| Blank | `3` | Riga vuota dopo ogni gruppo. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotLineTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Aggiungi campo riga e campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Ordina il campo riga per valori in ordine decrescente
            pivotTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "B2");
            
            // Calcola i dati della tabella pivot
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotLineTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


