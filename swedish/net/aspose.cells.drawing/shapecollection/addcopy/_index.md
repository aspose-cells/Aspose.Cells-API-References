---
title: "ShapeCollection.AddCopy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till och kopierar en form till arbetsbladet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addcopy/
---
## AddCopy(Shape, int, int, int, int) {#addcopy}

Lägger till och kopierar en shape i kalkylbladet.

```csharp
public Shape AddCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceShape | Form | Källform. |
| topRow | Int32 | Index för översta raden. |
| top | Int32 | Representerar det vertikala offsetet från dess översta rad, i enhet pixel. |
| leftColumn | Int32 | Det vänstra kolumnindexet. |
| vänster | Int32 | Representerar det horisontella offsetet från dess vänstra kolumn, i enhet pixel. |

### Returvärde

Det nya [`Shape`](../../shape/) objektet.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddCopyWithShapeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta samlingen av former
            ShapeCollection shapes = worksheet.Shapes;

            // Lägg till en rektangelform
            RectangleShape rectangle = shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Lägg till en kopia av rektangelformen med ny position
            shapes.AddCopy(rectangle, 7, 0, 7, 0);

            // Spara arbetsboken
            workbook.Save("ShapeCollectionMethodAddCopyDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(Shape, int, int, int, int, CopyOptions) {#addcopy_1}

Lägger till och kopierar en shape i kalkylbladet.

```csharp
public Shape AddCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, 
    CopyOptions copyOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceShape | Form | Källform. |
| topRow | Int32 | Index för översta raden. |
| top | Int32 | Representerar det vertikala offsetet från dess översta rad, i enhet pixel. |
| leftColumn | Int32 | Det vänstra kolumnindexet. |
| vänster | Int32 | Representerar det horisontella offsetet från dess vänstra kolumn, i enhet pixel. |
| copyOptions | CopyOptions | Alternativen för att kopiera former. |

### Returvärde

Det nya [`Shape`](../../shape/) objektet.

### Exempel

```csharp

[C#]
//lägg till en form
RectangleShape rectangle = shapes.AddRectangle(2, 0, 2, 0, 130, 130);
//Lägger till och kopierar en form.
shapes.AddCopy(rectangle, 7, 0, 7, 0);
```

### Se även

* class [Shape](../../shape/)
* class [CopyOptions](../../../aspose.cells/copyoptions/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


