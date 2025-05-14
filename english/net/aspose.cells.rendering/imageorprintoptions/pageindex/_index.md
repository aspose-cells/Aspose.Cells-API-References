---
title: ImageOrPrintOptions.PageIndex
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Gets or sets the 0based index of the first page to save
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/pageindex/
---
## ImageOrPrintOptions.PageIndex property

Gets or sets the 0-based index of the first page to save.

```csharp
public int PageIndex { get; set; }
```

### Remarks

Default is 0.

### Examples

```csharp
// Called: imgOpt.PageIndex = 1;
//Also for CELLSNET50088
public void ImageOrPrintOptions_Property_PageIndex()
{
    string destFile = Constants.destPath + "example.pdf";

    Workbook wb = new Workbook(Constants.TemplatePath + "example.xlsx");

    ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
    imgOpt.PrintWithStatusDialog = false;
    imgOpt.PageIndex = 1;
    imgOpt.PageCount = 1;

    PrinterSettings printerSettings = new PrinterSettings();
    printerSettings.PrintToFile = true;
    printerSettings.PrintFileName = destFile;
    printerSettings.PrinterName = "Microsoft Print to PDF";

    if (printerSettings.IsValid)
    {
        SheetRender sr = new SheetRender(wb.Worksheets[wb.Worksheets.ActiveSheetIndex], imgOpt);
        sr.ToPrinter(printerSettings, "test CELLSNET-50063 and CELLSNET-50088");

        //wait max 1s
        int count = 0;
        while (count < 10 && !File.Exists(destFile))
        {
            Thread.Sleep(1000);
            count++;
        }

        if (count < 10)
        {
            string content = File.ReadAllText(destFile);
            //only one page in pdf.
            Assert.IsTrue(content.IndexOf("/Count 1") > -1);
        }
    }
}
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


