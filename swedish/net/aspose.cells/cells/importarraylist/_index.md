---
title: "Cells.ImportArrayList"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Importerar en arraylist med data till ett kalkylblad"
type: docs
url: /sv/net/aspose.cells/cells/importarraylist/
---
## Cells.ImportArrayList method

Importerar en arraylist av data till ett kalkylblad.

```csharp
public void ImportArrayList(ArrayList arrayList, int firstRow, int firstColumn, bool isVertical)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arrayList | ArrayList | Data-arraylist. |
| firstRow | Int32 | Radnumret för den första cellen att importera i. |
| firstColumn | Int32 | Kolumnnumret för den första cellen att importera i. |
| ärVertikal | Boolean | Anger om data ska importeras vertikalt eller horisontellt. |

### Exempel

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportArrayListWithArrayListInt32Int32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            ArrayList data = new ArrayList();
            data.Add("Name");
            data.Add("Age");
            data.Add("City");
            
            cells.ImportArrayList(data, 0, 0, false);
            
            data.Clear();
            data.Add("John");
            data.Add(30);
            data.Add("New York");
            
            cells.ImportArrayList(data, 1, 0, false);
            
            workbook.Save("ImportArrayListDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


