---
title: "OleObject.ImageSourceFullName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OleObject egenskap. Hämtar eller anger sökväg och namn på källfilen för den länkade bilden"
type: docs
url: /sv/net/aspose.cells.drawing/oleobject/imagesourcefullname/
---
## OleObject.ImageSourceFullName property

Hämtar eller anger sökväg och namn för källfilen till den länkade bilden.

```csharp
public string ImageSourceFullName { get; set; }
```

### Anmärkningar

Standardvärdet är en tom sträng. Om SourceFullName inte är en tom sträng, länkas bilden. Om SourceFullName inte är en tom sträng, men Data är null, länkas bilden och lagras inte i filen.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyImageSourceFullNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempel på PDF-fil att bädda in
            byte[] pdfBytes = File.ReadAllBytes("example.pdf");

            // Lägg till ett OleObject i kalkylbladet
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, pdfBytes);
            OleObject oleObj = worksheet.OleObjects[oleIndex];

            // Ställ in OleObject-egenskaper inklusive ImageSourceFullName
            oleObj.DisplayAsIcon = false;
            oleObj.FileFormatType = FileFormatType.Pdf;
            oleObj.ImageSourceFullName = "sample_image.png"; // Demonstrating ImageSourceFullName usage
            oleObj.IsAutoSize = false;
            oleObj.IsLink = false;
            oleObj.ProgID = "Acrobat.Document.DC";

            // Spara arbetsboken
            workbook.Save("OleObjectDemo.xlsx");
        }
    }
}
```

### Se även

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


