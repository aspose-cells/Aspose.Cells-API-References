---
title: "PivotTable.CustomListSort"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se considerare l'elenco personalizzato incorporato durante l'ordinamento dei dati"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/customlistsort/
---
## PivotTable.CustomListSort property

Indica se considerare l'elenco personalizzato integrato durante l'ordinamento dei dati

```csharp
public bool CustomListSort { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyCustomListSortDemo
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
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Pear";
            cells["B5"].Value = 5;

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Aggiungi campo riga e campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Abilita l'ordinamento dell'elenco personalizzato
            pivotTable.CustomListSort = true;

            // Salva la cartella di lavoro
            workbook.Save("PivotTable_CustomListSort_Example.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


