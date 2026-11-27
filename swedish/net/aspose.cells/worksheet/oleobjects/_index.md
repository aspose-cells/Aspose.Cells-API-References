---
title: "Worksheet.OleObjects"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Kalkylbladsattribut. Representerar en samling av OleObject i ett kalkylblad"
type: docs
url: /sv/net/aspose.cells/worksheet/oleobjects/
---
## Worksheet.OleObjects property

Representerar en samling av [`OleObject`](../../../aspose.cells.drawing/oleobject/) i ett kalkylblad.

```csharp
public OleObjectCollection OleObjects { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett OleObject i kalkylbladet
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, File.ReadAllBytes(@"C:\temp\example.xlsx"));
            OleObject ole = worksheet.OleObjects[oleObjectIndex];
            
            // Ändra OleObject-egenskaper
            ole.ObjectSourceFullName = @"C:\temp\modified.xlsx";
            ole.FileFormatType = FileFormatType.Xlsx;

            // Spara arbetsboken
            workbook.Save(@"C:\temp\output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [OleObjectCollection](../../../aspose.cells.drawing/oleobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


