---
title: "Worksheet.OleObjects"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Stellt eine Sammlung von OleObject in einem Arbeitsblatt dar"
type: docs
url: /de/net/aspose.cells/worksheet/oleobjects/
---
## Worksheet.OleObjects property

Stellt eine Sammlung von [`OleObject`](../../../aspose.cells.drawing/oleobject/) in einem Arbeitsblatt dar.

```csharp
public OleObjectCollection OleObjects { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyOleObjectsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein OleObject zum Arbeitsblatt hinzufügen
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, File.ReadAllBytes(@"C:\temp\example.xlsx"));
            OleObject ole = worksheet.OleObjects[oleObjectIndex];
            
            // OleObject‑Eigenschaften ändern
            ole.ObjectSourceFullName = @"C:\temp\modified.xlsx";
            ole.FileFormatType = FileFormatType.Xlsx;

            // Speichere die Arbeitsmappe
            workbook.Save(@"C:\temp\output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [OleObjectCollection](../../../aspose.cells.drawing/oleobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


