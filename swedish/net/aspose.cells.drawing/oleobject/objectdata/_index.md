---
title: "OleObject.ObjectData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OleObject-egenskap. Representerar inbäddad ole-objektsdata som bytearray"
type: docs
url: /sv/net/aspose.cells.drawing/oleobject/objectdata/
---
## OleObject.ObjectData property

Representerar inbäddad ole-objektdata som bytearray.

```csharp
public byte[] ObjectData { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyObjectDataDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            var workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            var worksheet = workbook.Worksheets[0];
            
            // Exempel på filsökvägar (ersätt med faktiska sökvägar i din miljö)
            string imagePath = "logo.jpg";
            string oleDataPath = "test.xls";

            // Lägg till OLE-objekt med initial bilddata
            int oleIndex = worksheet.OleObjects.Add(10, 10, 300, 200, File.ReadAllBytes(imagePath));
            
            // Ändra OLE-objektets data
            worksheet.OleObjects[oleIndex].ObjectData = File.ReadAllBytes(oleDataPath);
            
            // Spara arbetsboken
            workbook.Save("OleObjectDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("OLE object demo created successfully.");
        }
    }
}
```

### Se även

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


