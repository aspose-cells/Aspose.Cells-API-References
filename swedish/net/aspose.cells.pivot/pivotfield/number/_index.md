---
title: "PivotField.Number"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-egenskap. Representerar det inbyggda visningsformatet för tal och datum"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/number/
---
## PivotField.Number property

Representerar det inbyggda visningsformatet för tal och datum.

```csharp
public int Number { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(new DateTime(2023, 1, 8));
            sheet.Cells["A3"].PutValue(new DateTime(2023, 1, 15));
            sheet.Cells["A4"].PutValue(new DateTime(2023, 1, 22));
            
            // Skapa pivottabell
            int pivotIndex = sheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            // Lägg till datumfält i kolumnområdet och ange talformat
            int fieldIndex = pivot.AddFieldToArea(PivotFieldType.Column, 0);
            PivotField field = pivot.ColumnFields[fieldIndex];
            field.Number = 16; // d-mmm format
            
            // Uppdatera och beräkna pivottabell
            pivot.RefreshData();
            pivot.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotFieldNumberDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


