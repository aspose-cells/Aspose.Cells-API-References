---
title: "PivotTable.PivotTableStyleType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Ottiene e imposta lo stile predefinito della tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/pivottablestyletype/
---
## PivotTable.PivotTableStyleType property

Ottiene e imposta lo stile predefinito della tabella pivot.

```csharp
public PivotTableStyleType PivotTableStyleType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPivotTableStyleTypeDemo
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
            cells["B4"].Value = 7;

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Imposta e dimostra PivotTableStyleType
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            Console.WriteLine("PivotTable Style Type: " + pivotTable.PivotTableStyleType);

            // Salva la cartella di lavoro
            workbook.Save("PivotTableStyleTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotTableStyleType](../../pivottablestyletype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


