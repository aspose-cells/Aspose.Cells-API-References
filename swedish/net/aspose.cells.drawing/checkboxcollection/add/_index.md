---
title: "CheckBoxCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CheckBoxCollection-metod. Lägger till en checkBox i samlingen"
type: docs
url: /sv/net/aspose.cells.drawing/checkboxcollection/add/
---
## CheckBoxCollection.Add method

Lägger till en checkBox i samlingen.

```csharp
public int Add(int topRow, int leftColumn, int height, int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| höjd | Int32 | Höjd på checkBox, i pixelenheter. |
| bredd | Int32 | Bredd på checkBox, i pixelenheter. |

### Returvärde

[`CheckBox`](../../checkbox/) object index.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxCollectionMethodAddWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till checkBox med Int32-parametrar (upperLeftRow, upperLeftColumn, height, width)
            int index = worksheet.CheckBoxes.Add(10, 2, 20, 100);
            
            CheckBox checkBox = worksheet.CheckBoxes[index];
            checkBox.Text = "Sample CheckBox";
            checkBox.Value = true;
            checkBox.LinkedCell = "B11";
            
            workbook.Save("CheckBoxDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


