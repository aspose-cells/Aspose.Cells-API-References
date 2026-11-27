---
title: "Protection.AllowUsingPivotTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Protection egenskap. Anger om användaren får manipulera pivottabeller på ett skyddat kalkylblad"
type: docs
url: /sv/net/aspose.cells/protection/allowusingpivottable/
---
## Protection.AllowUsingPivotTable property

Representerar om användaren får manipulera pivottabeller på ett skyddat kalkylblad.

```csharp
public bool AllowUsingPivotTable { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowUsingPivotTableDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aktivera skydd av kalkylblad
            Protection protection = worksheet.Protection;
            protection.AllowUsingPivotTable = true;
            worksheet.Protect(ProtectionType.All);

            // Verifiera inställningen
            Console.WriteLine("AllowUsingPivotTable is set to: " + protection.AllowUsingPivotTable);

            // Skapa en pivottabell för att demonstrera funktionaliteten
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);

            // Skapa pivottabell med korrekta parametrar
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "C1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Spara arbetsboken
            workbook.Save("ProtectionPropertyAllowUsingPivotTableDemo.xlsx");
        }
    }
}
```

### Se även

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


