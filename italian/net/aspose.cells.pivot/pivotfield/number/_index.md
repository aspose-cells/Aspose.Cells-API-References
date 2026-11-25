---
title: "PivotField.Number"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Rappresenta il formato di visualizzazione predefinito di numeri e date"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/number/
---
## PivotField.Number property

Rappresenta il formato di visualizzazione predefinito di numeri e date.

```csharp
public int Number { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyNumberDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(new DateTime(2023, 1, 8));
            sheet.Cells["A3"].PutValue(new DateTime(2023, 1, 15));
            sheet.Cells["A4"].PutValue(new DateTime(2023, 1, 22));
            
            // Crea tabella pivot
            int pivotIndex = sheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            // Aggiungi un campo data all'area colonne e imposta il formato numerico
            int fieldIndex = pivot.AddFieldToArea(PivotFieldType.Column, 0);
            PivotField field = pivot.ColumnFields[fieldIndex];
            field.Number = 16; // d-mmm format
            
            // Aggiorna e calcola la tabella pivot
            pivot.RefreshData();
            pivot.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFieldNumberDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


