---
title: "PivotTable.IsGridDropZones"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se il report della PivotTable visualizza il layout classico della tabella pivot. abilita il trascinamento dei campi nella griglia"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/isgriddropzones/
---
## PivotTable.IsGridDropZones property

Indica se il report PivotTable visualizza il layout classico della PivotTable. (consente il trascinamento dei campi nella griglia)

```csharp
public bool IsGridDropZones { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsGridDropZonesDemo
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
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Aggiungi tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Imposta la proprietà IsGridDropZones
            pivotTable.IsGridDropZones = true;
            Console.WriteLine("IsGridDropZones: " + pivotTable.IsGridDropZones);

            // Salva la cartella di lavoro
            workbook.Save("PivotTable_IsGridDropZones_Example.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


