---
title: "ShapeCollection.AddRadioButton"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till en RadioButton i kalkylbladet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addradiobutton/
---
## ShapeCollection.AddRadioButton method

Lägger till en radioknapp i kalkylbladet.

```csharp
public RadioButton AddRadioButton(int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| top | Int32 | Representerar det vertikala offsetet för RadioButton från dess vänstra rad, i enhet pixel. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| vänster | Int32 | Representerar den horisontella förskjutningen av RadioButton från dess vänstra kolumn, i enhet pixel. |
| höjd | Int32 | Representerar höjden på RadioButton, i enhet pixel. |
| bredd | Int32 | Representerar bredden på RadioButton, i enhet pixel. |

### Returvärde

Ett RadioButton-objekt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddRadioButtonWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en radioknapp i kalkylbladet
            Aspose.Cells.Drawing.RadioButton radioButton = worksheet.Shapes.AddRadioButton(1, 0, 1, 0, 100, 50);
            radioButton.Text = "Option 1";

            // Spara arbetsboken
            workbook.Save("RadioButtonDemo.xlsx");
        }
    }
}
```

### Se även

* class [RadioButton](../../radiobutton/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


