---
title: "Enum SlicerStyleType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Slicers.SlicerStyleType-enum. Ange stilen för skivkontrollens vy"
type: docs
url: /sv/net/aspose.cells.slicers/slicerstyletype/
---
## SlicerStyleType enumeration

Specificera stilen för slicer-vyn.

```csharp
public enum SlicerStyleType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| SlicerStyleLight1 | `0` | inbyggd ljus stil ett |
| SlicerStyleLight2 | `1` | inbyggd ljus stil två |
| SlicerStyleLight3 | `2` | inbyggd ljus stil tre |
| SlicerStyleLight4 | `3` | inbyggd ljus stil fyra |
| SlicerStyleLight5 | `4` | inbyggd ljus stil fem |
| SlicerStyleLight6 | `5` | inbyggd ljus stil sex |
| SlicerStyleOther1 | `6` | inbyggd stil annan ett |
| SlicerStyleOther2 | `7` | inbyggd stil annan två |
| SlicerStyleDark1 | `8` | inbyggd mörk stil ett |
| SlicerStyleDark2 | `9` | inbyggd mörk stil två |
| SlicerStyleDark3 | `10` | inbyggd mörk stil tre |
| SlicerStyleDark4 | `11` | inbyggd mörk stil fyra |
| SlicerStyleDark5 | `12` | inbyggd mörk stil fem |
| SlicerStyleDark6 | `13` | inbyggd mörk stil sex |
| Custom | `14` | användardefinierad stil, för närvarande ej stödd |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicersClassSlicerStyleTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Skapa exempeldata för pivottabell
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["A5"].Value = "Apple";
            sheet.Cells["B1"].Value = "Quantity";
            sheet.Cells["B2"].Value = 10;
            sheet.Cells["B3"].Value = 15;
            sheet.Cells["B4"].Value = 8;
            sheet.Cells["B5"].Value = 12;

            // Skapa pivottabell
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Lägg till skärmningskontrollen
            int slicerIndex = sheet.Slicers.Add(pivot, "G1", pivot.BaseFields[0]);
            Slicer slicer = sheet.Slicers[slicerIndex];
            
            // Ange slicer-stil
            slicer.StyleType = SlicerStyleType.SlicerStyleDark1;
            slicer.NumberOfColumns = 2;

            // Spara arbetsboken
            wb.Save("SlicerStyleTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


