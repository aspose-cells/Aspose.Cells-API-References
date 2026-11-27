---
title: "MsoFormatPicture.IsGray"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFormatPicture‑egenskap. Anger om bilden ska visas i gråskala"
type: docs
url: /sv/net/aspose.cells.drawing/msoformatpicture/isgray/
---
## MsoFormatPicture.IsGray property

Indikerar om den här bilden ska visas i gråskala.

```csharp
public bool IsGray { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyIsGrayDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bildform
            using (Stream imageStream = File.OpenRead("example.gif"))
            {
                Shape shape = worksheet.Shapes.AddPicture(0, 0, imageStream, 100, 100);
                
                // Ange bildformatets egenskaper
                shape.FormatPicture.Brightness = 90;
                shape.FormatPicture.Contrast = 90;
                shape.FormatPicture.IsGray = true;

                // Spara arbetsboken
                workbook.Save("output.xlsx");
            }

            // Läs in igen och verifiera egenskaperna
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            
            Console.WriteLine("Brightness: " + loadedShape.FormatPicture.Brightness);
            Console.WriteLine("Contrast: " + loadedShape.FormatPicture.Contrast);
            Console.WriteLine("IsGray: " + loadedShape.FormatPicture.IsGray);
        }
    }
}
```

### Se även

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


