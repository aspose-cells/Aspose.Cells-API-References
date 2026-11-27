---
title: "OleObject.IsAutoSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OleObject-egenskap. True indikerar att storleken på ole-objektet automatiskt kommer att ändras till storleken på en ögonblicksbild av det inbäddade innehållet när ole-objektet aktiveras"
type: docs
url: /sv/net/aspose.cells.drawing/oleobject/isautosize/
---
## OleObject.IsAutoSize property

Sant indikerar att storleken på OLE-objektet automatiskt ändras till storleken på en ögonblicksbild av det inbäddade innehållet när OLE-objektet aktiveras.

```csharp
public bool IsAutoSize { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett OLE-objekt (använder fildata som byte array)
            byte[] oleData = System.IO.File.ReadAllBytes(@"C:\example\test.docx");
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, oleData);
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleIndex];

            // Ställ in och demonstrera IsAutoSize-egenskapen
            oleObject.IsAutoSize = true;
            Console.WriteLine("OLE Object AutoSize initially: " + oleObject.IsAutoSize);

            // Ändra egenskapen
            oleObject.IsAutoSize = false;
            Console.WriteLine("OLE Object AutoSize after change: " + oleObject.IsAutoSize);

            // Spara arbetsboken
            workbook.Save("OleObjectIsAutoSizeDemo.xlsx");
        }
    }
}
```

### Se även

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


