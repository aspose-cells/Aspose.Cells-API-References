---
title: "ShapeCollection.AddComboBox"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt ein ComboBox zum Arbeitsblatt hinzu"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addcombobox/
---
## ShapeCollection.AddComboBox method

Fügt eine ComboBox zum Arbeitsblatt hinzu.

```csharp
public ComboBox AddComboBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| oben | Int32 | Stellt den vertikalen Versatz des ComboBox von seiner linken Zeile dar, in Pixel. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| links | Int32 | Stellt den horizontalen Versatz des ComboBox von seiner linken Spalte dar, in Pixel. |
| Höhe | Int32 | Stellt die Höhe des ComboBox dar, in Pixel. |
| Breite | Int32 | Stellt die Breite des ComboBox dar, in Pixel. |

### Rückgabewert

Ein ComboBox-Objekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddComboBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rufe die Formensammlung ab
            ShapeCollection shapes = worksheet.Shapes;

            // Fügen Sie ein ComboBox mit angegebenen Parametern hinzu
            Aspose.Cells.Drawing.ComboBox comboBox = shapes.AddComboBox(1, 0, 1, 0, 100, 50);

            // Fügen Sie dem ComboBox Elemente hinzu, indem Sie Zellwerte festlegen
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Legen Sie den Eingabebereich für das Kombinationsfeld fest
            comboBox.InputRange = "A1:A3";
            comboBox.DropDownLines = 3;

            // Speichere die Arbeitsmappe
            workbook.Save("AddComboBoxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ComboBox](../../combobox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


