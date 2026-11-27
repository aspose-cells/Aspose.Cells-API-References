---
title: "Cell.Characters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Returnerar ett Characters-objekt som representerar ett teckenintervall inom cellens text"
type: docs
url: /sv/net/aspose.cells/cell/characters/
---
## Cell.Characters method

Returnerar ett Characters-objekt som representerar ett teckenintervall inom cellens text.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | Int32 | Indexet för början av tecknet. |
| length | Int32 | Antalet tecken. |

### Returvärde

Characters-objekt.

### Anmärkningar

Denna metod fungerar endast på cellen med strängvärde.

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["A1"].PutValue("Helloworld");
            cells["A1"].Characters(5, 5).Font.IsBold = true;
            cells["A1"].Characters(5, 5).Font.Color = Color.Blue;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


