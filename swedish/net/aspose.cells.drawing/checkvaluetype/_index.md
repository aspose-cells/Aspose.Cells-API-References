---
title: "Enum CheckValueType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.CheckValueType enum. Representerar kryssvärdestypen för kryssrutan"
type: docs
url: /sv/net/aspose.cells.drawing/checkvaluetype/
---
## CheckValueType enumeration

Representerar kryssvärdestypen för kryssrutan.

```csharp
public enum CheckValueType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| UnChecked | `0` | Ej markerad |
| Checked | `1` | Markerad |
| Mixed | `2` | Blandad |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassCheckValueTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till kryssrutor i kalkylbladet
            int checkboxIndex1 = sheet.CheckBoxes.Add(0, 0, 100, 100);
            int checkboxIndex2 = sheet.CheckBoxes.Add(0, 1, 100, 100);

            // Hämta kryssrutorna och ställ in deras egenskaper
            Aspose.Cells.Drawing.CheckBox checkbox1 = sheet.CheckBoxes[checkboxIndex1];
            Aspose.Cells.Drawing.CheckBox checkbox2 = sheet.CheckBoxes[checkboxIndex2];

            // Ställ in kryssrutornas värden och markeringsstatus
            checkbox1.Value = true;
            checkbox1.CheckedValue = CheckValueType.Checked;
            
            checkbox2.Value = false;
            checkbox2.CheckedValue = CheckValueType.UnChecked;  // Note: Changed from Unchecked to UnChecked

            // Länka kryssrutor till celler
            checkbox1.LinkedCell = "A1";
            checkbox2.LinkedCell = "A2";

            // Skriv ut cellvärdena för att demonstrera länken
            Console.WriteLine("Cell A1 value (should be true): " + sheet.Cells["A1"].BoolValue);
            Console.WriteLine("Cell A2 value (should be false): " + sheet.Cells["A2"].BoolValue);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


