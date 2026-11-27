---
title: "OleObject.ClassIdentifier"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OleObject-egenskap. Hämtar och anger klassidentifieraren för det inbäddade objektet. Det betyder vilken applikation som öppnar den inbäddade filen"
type: docs
url: /sv/net/aspose.cells.drawing/oleobject/classidentifier/
---
## OleObject.ClassIdentifier property

Hämtar och anger klassidentifieraren för det inbäddade objektet. Det betyder vilket program som öppnar den inbäddade filen.

```csharp
public byte[] ClassIdentifier { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyClassIdentifierDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Exempel på byte array för ClassIdentifier (vanligtvis skulle detta vara ett riktigt klass-ID)
            byte[] classId = new byte[] { 0x01, 0x02, 0x03, 0x04, 0x05, 0x06, 0x07, 0x08, 
                                         0x09, 0x0A, 0x0B, 0x0C, 0x0D, 0x0E, 0x0F, 0x10 };

            // Lägg till ett OLE-objekt med exempeldata
            int oleIndex = sheet.OleObjects.Add(10, 10, 200, 100, new byte[100]);
            OleObject oleObject = sheet.OleObjects[oleIndex];
            
            // Ange ClassIdentifier-egenskapen
            oleObject.ClassIdentifier = classId;
            oleObject.ProgID = "Excel.Sheet.12";
            oleObject.DisplayAsIcon = true;

            // Spara arbetsboken
            workbook.Save("OleObjectDemo.xlsx");

            // Läs in den sparade arbetsboken för att verifiera ClassIdentifier
            Workbook loadedWorkbook = new Workbook("OleObjectDemo.xlsx");
            OleObject loadedOle = loadedWorkbook.Worksheets[0].OleObjects[0];
            
            // Verifiera att ClassIdentifier bevarades
            Console.WriteLine("ClassIdentifier length: " + loadedOle.ClassIdentifier.Length);
        }
    }
}
```

### Se även

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


