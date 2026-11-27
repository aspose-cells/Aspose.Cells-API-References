---
title: "OleObject.AutoLoad"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OleObject-egenskap. Anger om värdapplikationen för det inbäddade objektet ska anropas för att automatiskt ladda objektdata när den överordnade arbetsboken öppnas"
type: docs
url: /sv/net/aspose.cells.drawing/oleobject/autoload/
---
## OleObject.AutoLoad property

Anger om värdprogrammet för det inbäddade objektet ska anropas för att automatiskt läsa in objektdata när den överordnade arbetsboken öppnas.

```csharp
public bool AutoLoad { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyAutoLoadDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till ett OleObject i kalkylbladet
            int oleNumber = sheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            
            // Ange OleObject-egenskaper
            OleObject ole = sheet.OleObjects[oleNumber];
            ole.ProgID = "Excel.Sheet";
            ole.ObjectData = new byte[0];
            
            // Demonstrera AutoLoad-egenskapen
            ole.AutoLoad = true; // Automatically load the OleObject when the workbook opens
            
            // Spara arbetsboken
            workbook.Save("OleObjectAutoLoadDemo.xlsx");
        }
    }
}
```

### Se även

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


