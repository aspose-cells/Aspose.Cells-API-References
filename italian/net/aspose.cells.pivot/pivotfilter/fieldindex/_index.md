---
title: "PivotFilter.FieldIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotFilter property. Ottiene l'indice del campo sorgente a cui è applicato questo filtro pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotfilter/fieldindex/
---
## PivotFilter.FieldIndex property

Ottiene l'indice del campo sorgente a cui è applicato questo filtro pivot.

```csharp
public int FieldIndex { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyFieldIndexDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 8;

            // Aggiungi tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Aggiungi campo riga e campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Aggiungi filtro
            pivotTable.AddFieldToArea(PivotFieldType.Page, 0);
            PivotField pivotField = pivotTable.PageFields[0];
            
            // Crea una collezione di filtri pivot e aggiungi filtro
            PivotFilterCollection filters = pivotTable.PivotFilters;
            int filterIndex = filters.Add(0, PivotFilterType.Count);
            PivotFilter filter = filters[filterIndex];
            
            // Dimostra la proprietà FieldIndex
            Console.WriteLine("Field Index: " + filter.FieldIndex);

            // Salva la cartella di lavoro
            workbook.Save("PivotFilterFieldIndexDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


