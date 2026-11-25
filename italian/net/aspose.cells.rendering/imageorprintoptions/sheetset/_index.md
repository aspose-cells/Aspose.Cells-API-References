---
title: "ImageOrPrintOptions.SheetSet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Ottiene o imposta i fogli da renderizzare. Il valore predefinito è tutti i fogli visibili nella cartella di lavoro Visible"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/sheetset/
---
## ImageOrPrintOptions.SheetSet property

Ottiene o imposta i fogli da renderizzare. Il valore predefinito è tutti i fogli visibili nella cartella di lavoro: [`Visible`](../../sheetset/visible/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Osservazioni

Il set è ignorato quando viene utilizzato in [`SheetRender`](../../sheetrender/)

### Esempi

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
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "VisibleSheet1";
            sheet1.Cells["A1"].PutValue("Sheet1 Content");
            
            Worksheet sheet2 = workbook.Worksheets.Add("VisibleSheet2");
            sheet2.Cells["A1"].PutValue("Sheet2 Content");
            
            Worksheet sheet3 = workbook.Worksheets.Add("HiddenSheet");
            sheet3.Cells["A1"].PutValue("Hidden Content");
            sheet3.IsVisible = false;

            // Dimostrare la proprietà SheetSet con ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;

            // Opzione 1: Stampare tutti i fogli (inclusi quelli nascosti)
            options.SheetSet = SheetSet.All;
            WorkbookRender allSheetsRender = new WorkbookRender(workbook, options);
            Console.WriteLine($"All sheets page count: {allSheetsRender.PageCount}");

            // Opzione 2: Stampare solo i fogli visibili
            options.SheetSet = SheetSet.Visible;
            WorkbookRender visibleSheetsRender = new WorkbookRender(workbook, options);
            Console.WriteLine($"Visible sheets page count: {visibleSheetsRender.PageCount}");

            // Opzione 3: Stampare fogli specifici per indice
            options.SheetSet = new SheetSet(new int[] { 0, 2 }); // First and third sheets
            WorkbookRender specificSheetsRender = new WorkbookRender(workbook, options);
            Console.WriteLine($"Specific sheets page count: {specificSheetsRender.PageCount}");

            // Salvare una pagina nello stream come dimostrazione
            using (MemoryStream stream = new MemoryStream())
            {
                specificSheetsRender.ToImage(0, stream);
                Console.WriteLine($"Image stream length: {stream.Length} bytes");
            }
        }
    }
}
```

### Vedi anche

* class [SheetSet](../../sheetset/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


