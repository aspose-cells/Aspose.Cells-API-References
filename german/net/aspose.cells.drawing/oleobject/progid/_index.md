---
title: "OleObject.ProgID"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OleObject-Eigenschaft. Liest oder setzt die ProgID des OLE-Objekts"
type: docs
url: /de/net/aspose.cells.drawing/oleobject/progid/
---
## OleObject.ProgID property

Liest oder setzt die ProgID des OLE-Objekts.

```csharp
public string ProgID { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein OLE-Objekt zum Arbeitsblatt hinzufügen
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0], "test.pdf");
            OleObject ole = worksheet.OleObjects[oleIndex];
            
            // ProgID für das OLE-Objekt festlegen
            ole.ProgID = "AcroExch.Document.DC";
            
            // ProgID anzeigen
            Console.WriteLine("OLE Object ProgID: " + ole.ProgID);

            // Speichere die Arbeitsmappe
            workbook.Save("OleObjectProgIDDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


