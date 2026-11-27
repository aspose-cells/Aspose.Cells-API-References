---
title: "OleObject.ProgID"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OleObject-egenskap. Hämtar eller anger ProgID för OLE-objektet"
type: docs
url: /sv/net/aspose.cells.drawing/oleobject/progid/
---
## OleObject.ProgID property

Hämtar eller anger ProgID för OLE-objektet.

```csharp
public string ProgID { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyProgIDDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett OLE‑objekt i kalkylbladet
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0], "test.pdf");
            OleObject ole = worksheet.OleObjects[oleIndex];
            
            // Ange ProgID för OLE-objektet
            ole.ProgID = "AcroExch.Document.DC";
            
            // Visa ProgID
            Console.WriteLine("OLE Object ProgID: " + ole.ProgID);

            // Spara arbetsboken
            workbook.Save("OleObjectProgIDDemo.xlsx");
        }
    }
}
```

### Se även

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


