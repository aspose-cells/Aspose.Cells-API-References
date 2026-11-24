---
title: "CheckBoxCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CheckBoxCollection-Methode. Fügt ein CheckBox zur Sammlung hinzu"
type: docs
url: /de/net/aspose.cells.drawing/checkboxcollection/add/
---
## CheckBoxCollection.Add method

Fügt der Sammlung ein checkBox hinzu.

```csharp
public int Add(int topRow, int leftColumn, int height, int width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| Höhe | Int32 | Höhe des CheckBox, in Pixel. |
| Breite | Int32 | Breite des CheckBox, in Pixel. |

### Rückgabewert

[`CheckBox`](../../checkbox/) object index.

### Beispiele

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

            // Fügen Sie ein CheckBox mit Int32-Parametern hinzu (upperLeftRow, upperLeftColumn, height, width)
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

### Siehe auch

* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


