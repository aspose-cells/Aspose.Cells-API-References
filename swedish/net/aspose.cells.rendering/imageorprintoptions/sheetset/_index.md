---
title: "ImageOrPrintOptions.SheetSet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Hämtar eller anger bladen som ska renderas. Standard är alla synliga blad i arbetsboken Visible"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/sheetset/
---
## ImageOrPrintOptions.SheetSet property

Hämtar eller anger bladen som ska renderas. Standard är alla synliga blad i arbetsboken: [`Visible`](../../sheetset/visible/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Anmärkningar

Uppsättningen ignoreras när den används i [`SheetRender`](../../sheetrender/)

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "VisibleSheet1";
            sheet1.Cells["A1"].PutValue("Sheet1 Content");
            
            Worksheet sheet2 = workbook.Worksheets.Add("VisibleSheet2");
            sheet2.Cells["A1"].PutValue("Sheet2 Content");
            
            Worksheet sheet3 = workbook.Worksheets.Add("HiddenSheet");
            sheet3.Cells["A1"].PutValue("Hidden Content");
            sheet3.IsVisible = false;

            // Demonstrera SheetSet-egenskap med ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;

            // Alternativ 1: Skriv ut alla blad (inklusive dolda)
            options.SheetSet = SheetSet.All;
            WorkbookRender allSheetsRender = new WorkbookRender(workbook, options);
            Console.WriteLine($"All sheets page count: {allSheetsRender.PageCount}");

            // Alternativ 2: Skriv ut endast synliga blad
            options.SheetSet = SheetSet.Visible;
            WorkbookRender visibleSheetsRender = new WorkbookRender(workbook, options);
            Console.WriteLine($"Visible sheets page count: {visibleSheetsRender.PageCount}");

            // Alternativ 3: Skriv ut specifika blad efter index
            options.SheetSet = new SheetSet(new int[] { 0, 2 }); // First and third sheets
            WorkbookRender specificSheetsRender = new WorkbookRender(workbook, options);
            Console.WriteLine($"Specific sheets page count: {specificSheetsRender.PageCount}");

            // Spara en sida till ström som demonstration
            using (MemoryStream stream = new MemoryStream())
            {
                specificSheetsRender.ToImage(0, stream);
                Console.WriteLine($"Image stream length: {stream.Length} bytes");
            }
        }
    }
}
```

### Se även

* class [SheetSet](../../sheetset/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


