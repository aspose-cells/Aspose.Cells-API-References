---
title: "Worksheet.CheckBoxes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar en CheckBox‑samling"
type: docs
url: /sv/net/aspose.cells/worksheet/checkboxes/
---
## Worksheet.CheckBoxes property

Hämtar en [`CheckBox`](../../../aspose.cells.drawing/checkbox/) samling.

```csharp
public CheckBoxCollection CheckBoxes { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCheckBoxesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till tre checkboxes med olika egenskaper
            int index1 = sheet.CheckBoxes.Add(10, 10, 20, 100);
            Aspose.Cells.Drawing.CheckBox checkBox1 = sheet.CheckBoxes[index1];
            checkBox1.Text = "Option 1";
            checkBox1.Value = true;

            int index2 = sheet.CheckBoxes.Add(40, 10, 20, 100);
            Aspose.Cells.Drawing.CheckBox checkBox2 = sheet.CheckBoxes[index2];
            checkBox2.Text = "Option 2";
            checkBox2.LinkedCell = "A1";

            int index3 = sheet.CheckBoxes.Add(70, 10, 20, 100);
            Aspose.Cells.Drawing.CheckBox checkBox3 = sheet.CheckBoxes[index3];
            checkBox3.Text = "Option 3";
            checkBox3.Value = true;

            workbook.Save("CheckBoxesDemo.xlsx");
        }
    }
}
```

### Se även

* class [CheckBoxCollection](../../../aspose.cells.drawing/checkboxcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


