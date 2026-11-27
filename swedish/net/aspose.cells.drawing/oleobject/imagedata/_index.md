---
title: "OleObject.ImageData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OleObject-egenskap. Representerar bilden av ole-objektet som byte array"
type: docs
url: /sv/net/aspose.cells.drawing/oleobject/imagedata/
---
## OleObject.ImageData property

Representerar bilden av ole-objektet som en bytearray.

```csharp
public byte[] ImageData { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyImageDataDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Läs bildfil till byte array
            byte[] imageBytes = File.ReadAllBytes("image1.png");
            
            // Lägg till OLE-objekt med bilddata
            int oleIndex = workbook.Worksheets[0].OleObjects.Add(0, 0, 60, 60, imageBytes);
            OleObject oleObject = workbook.Worksheets[0].OleObjects[oleIndex];
            
            // Ställ in egenskaper för inbäddat objekt
            oleObject.SetEmbeddedObject(false, imageBytes, "image1.png", true, "Sample Image", false);
            
            // Demonstrera användning av ImageData-egenskapen
            Console.WriteLine($"Image data length: {oleObject.ImageData.Length}");
            Console.WriteLine($"First byte: {oleObject.ImageData[0]}");
            Console.WriteLine($"Middle byte: {oleObject.ImageData[oleObject.ImageData.Length/2]}");
            Console.WriteLine($"Last byte: {oleObject.ImageData[oleObject.ImageData.Length-1]}");
            
            // Spara arbetsboken
            workbook.Save("OleObjectWithImage.xlsx");
        }
    }
}
```

### Se även

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


