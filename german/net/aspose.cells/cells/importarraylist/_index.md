---
title: "Cells.ImportArrayList"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Importiert eine ArrayList von Daten in ein Arbeitsblatt"
type: docs
url: /de/net/aspose.cells/cells/importarraylist/
---
## Cells.ImportArrayList method

Importiert eine ArrayList von Daten in ein Arbeitsblatt.

```csharp
public void ImportArrayList(ArrayList arrayList, int firstRow, int firstColumn, bool isVertical)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arrayList | ArrayList | Daten-ArrayList. |
| firstRow | Int32 | Die Zeilennummer der ersten Zelle, in die importiert werden soll. |
| firstColumn | Int32 | Die Spaltennummer der ersten Zelle, in die importiert werden soll. |
| isVertical | Boolean | Gibt an, ob Daten vertikal oder horizontal importiert werden sollen. |

### Beispiele

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

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


