---
title: "Cells.IsColumnHidden"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Kontrollerar om en kolumn på angivet index är dold"
type: docs
url: /sv/net/aspose.cells/cells/iscolumnhidden/
---
## Cells.IsColumnHidden method

Kontrollerar om en kolumn på angivet index är dold.

```csharp
public bool IsColumnHidden(int columnIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | Int32 | kolumnindex |

### Returvärde

sant om kolumnen är dold.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsColumnHiddenWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Dölj kolumn C (index 2)
            cells.HideColumn(2);
            
            // Kontrollera om kolumn C är dold
            bool isHidden = cells.IsColumnHidden(2);
            
            Console.WriteLine("Is column C (index 2) hidden? " + isHidden);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


