---
title: "OleObject.FileFormatType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OleObject egenskap. Hämtar och anger filtypen för den inbäddade ole-objektdata"
type: docs
url: /sv/net/aspose.cells.drawing/oleobject/fileformattype/
---
## OleObject.FileFormatType property

Hämtar och anger filtypen för den inbäddade ole-objektdatan

```csharp
public FileFormatType FileFormatType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyFileFormatTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till ett OLE-objekt i kalkylbladet (utan fildata)
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, null);
            
            // Hämta det tillagda OLE-objektet
            OleObject oleObject = worksheet.OleObjects[oleIndex];
            
            // Ställ in och visa filformatstypen
            oleObject.FileFormatType = FileFormatType.Docm;
            Console.WriteLine("OLE Object File Format Type: " + oleObject.FileFormatType);
            
            // Spara arbetsboken
            workbook.Save("OleObjectFileFormatTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [FileFormatType](../../../aspose.cells/fileformattype/)
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


