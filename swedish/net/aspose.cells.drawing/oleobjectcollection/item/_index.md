---
title: "OleObjectCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OleObjectCollection-egenskap. Hämtar OleObject-elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells.drawing/oleobjectcollection/item/
---
## OleObjectCollection indexer

Hämtar [`OleObject`](../../oleobject/) elementet på det angivna indexet.

```csharp
public OleObject this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till exempelbilddata
            byte[] binaryImg = File.ReadAllBytes("image1.png");
            
            // Lägg till OLE-objekt till det första kalkylbladet
            int idxOle = workbook.Worksheets[0].OleObjects.Add(0, 0, 60, 60, binaryImg);
            
            // Åtkomst till OLE-objektet med Item‑egenskapen
            OleObject objOle = workbook.Worksheets[0].OleObjects[idxOle];
            
            // Ställ in egenskaper för inbäddat objekt
            byte[] binaryXlsx = File.ReadAllBytes("example.xlsx");
            objOle.SetEmbeddedObject(false, binaryXlsx, "SampleFile.xlsx", true, "Excel.Sheet", false);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Verifiera den sparade filen
            Workbook savedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("OLE Object Source: " + savedWorkbook.Worksheets[0].OleObjects[0].ObjectSourceFullName);
        }
    }
}
```

### Se även

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


