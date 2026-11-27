---
title: "Cell.InsertText"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Infoga några tecken i cellen. Om cellen är rik formaterad kan denna metod behålla den ursprungliga formateringen"
type: docs
url: /sv/net/aspose.cells/cell/inserttext/
---
## Cell.InsertText method

Infoga några tecken i cellen. Om cellen är rik formaterad kan den här metoden behålla den ursprungliga formateringen.

```csharp
public void InsertText(int index, string text)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Indexet. |
| text | String | Infogad text. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodInsertTextWithInt32StringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Kom åt cell B3 och sätt initialt värde
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("OriginalText");
            
            // Infoga text på position 6
            cell.InsertText(6, "Inserted");
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


