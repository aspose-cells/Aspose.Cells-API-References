---
title: "ImageOrPrintOptions.SheetSet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Gibt die zu rendernden Arbeitsblätter zurück oder legt sie fest. Standard ist alle sichtbaren Arbeitsblätter in der Arbeitsmappe Visible"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/sheetset/
---
## ImageOrPrintOptions.SheetSet property

Gibt die zu rendernden Arbeitsblätter zurück oder legt sie fest. Standard ist alle sichtbaren Arbeitsblätter in der Arbeitsmappe: [`Visible`](../../sheetset/visible/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Hinweise

Der Satz wird ignoriert, wenn er in [`SheetRender`](../../sheetrender/) verwendet wird

### Beispiele

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
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "VisibleSheet1";
            sheet1.Cells["A1"].PutValue("Sheet1 Content");
            
            Worksheet sheet2 = workbook.Worksheets.Add("VisibleSheet2");
            sheet2.Cells["A1"].PutValue("Sheet2 Content");
            
            Worksheet sheet3 = workbook.Worksheets.Add("HiddenSheet");
            sheet3.Cells["A1"].PutValue("Hidden Content");
            sheet3.IsVisible = false;

            // Demonstration der SheetSet-Eigenschaft mit ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;

            // Option 1: Alle Arbeitsblätter drucken (einschließlich versteckter)
            options.SheetSet = SheetSet.All;
            WorkbookRender allSheetsRender = new WorkbookRender(workbook, options);
            Console.WriteLine($"All sheets page count: {allSheetsRender.PageCount}");

            // Option 2: Nur sichtbare Arbeitsblätter drucken
            options.SheetSet = SheetSet.Visible;
            WorkbookRender visibleSheetsRender = new WorkbookRender(workbook, options);
            Console.WriteLine($"Visible sheets page count: {visibleSheetsRender.PageCount}");

            // Option 3: Bestimmte Arbeitsblätter nach Index drucken
            options.SheetSet = new SheetSet(new int[] { 0, 2 }); // First and third sheets
            WorkbookRender specificSheetsRender = new WorkbookRender(workbook, options);
            Console.WriteLine($"Specific sheets page count: {specificSheetsRender.PageCount}");

            // Eine Seite als Demonstration in einen Stream speichern
            using (MemoryStream stream = new MemoryStream())
            {
                specificSheetsRender.ToImage(0, stream);
                Console.WriteLine($"Image stream length: {stream.Length} bytes");
            }
        }
    }
}
```

### Siehe auch

* class [SheetSet](../../sheetset/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


