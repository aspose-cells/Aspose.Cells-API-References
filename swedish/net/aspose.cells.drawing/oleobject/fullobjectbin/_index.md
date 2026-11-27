---
title: "OleObject.FullObjectBin"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OleObject egenskap. Hämtar hela den inbäddade ole‑objektets binära data i mallfilen"
type: docs
url: /sv/net/aspose.cells.drawing/oleobject/fullobjectbin/
---
## OleObject.FullObjectBin property

Hämtar den fullständiga binära datan för det inbäddade ole-objektet i mallfilen.

```csharp
public byte[] FullObjectBin { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectPropertyFullObjectBinDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett OLE‑objekt i kalkylbladet
            byte[] objectData = File.ReadAllBytes("example.docx");
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, objectData, "docx");
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            // Ange några egenskaper för OLE‑objektet
            oleObject.FileFormatType = FileFormatType.Docx;
            oleObject.ObjectData = objectData;
            oleObject.IsAutoSize = true;

            // Hämta FullObjectBin‑data (skrivskyddad egenskap)
            byte[] fullObjectBinData = oleObject.FullObjectBin;
            Console.WriteLine("FullObjectBin data length: " + (fullObjectBinData != null ? fullObjectBinData.Length.ToString() : "null"));

            // Demonstrera användning av FullObjectBin genom att spara den till en fil
            if (fullObjectBinData != null && fullObjectBinData.Length > 0)
            {
                File.WriteAllBytes("FullObjectBinData.bin", fullObjectBinData);
                Console.WriteLine("Saved FullObjectBin data to file.");
            }

            // Skapa en annan arbetsbok för att demonstrera läsning av OLE‑objektet
            Workbook workbook2 = new Workbook();
            Worksheet worksheet2 = workbook2.Worksheets[0];

            // Lägg till OLE‑objektet från FullObjectBin‑data
            if (fullObjectBinData != null)
            {
                int newOleObjectIndex = worksheet2.OleObjects.Add(10, 10, 200, 200, fullObjectBinData, "docx");
                Console.WriteLine("Added new OLE object using FullObjectBin data.");
            }

            // Spara arbetsböckerna
            workbook.Save("OleObjectWithFullObjectBin.xlsx");
            workbook2.Save("OleObjectFromFullObjectBin.xlsx");
        }
    }
}
```

### Se även

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


