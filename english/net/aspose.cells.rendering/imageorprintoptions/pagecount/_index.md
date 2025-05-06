---
title: ImageOrPrintOptions.PageCount
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Gets or sets the number of pages to save
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/pagecount/
---
## ImageOrPrintOptions.PageCount property

Gets or sets the number of pages to save.

```csharp
public int PageCount { get; set; }
```

### Remarks

Default is System.Int32.MaxValue which means all pages will be rendered.

### Examples

```csharp
// Called: imgOpt.PageCount = 1;
[Test]
        //Also for CELLSNET50088
        public void Property_PageCount()
        {
            string destFile = Constants.destPath + &quot;CELLSNET-50063.pdf&quot;;

            Workbook wb = new Workbook(Constants.TemplatePath + &quot;CELLSNET-50063.xlsx&quot;);

            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.PrintWithStatusDialog = false;
            imgOpt.PageIndex = 1;
            imgOpt.PageCount = 1;

            PrinterSettings printerSettings = new PrinterSettings();
            printerSettings.PrintToFile = true;
            printerSettings.PrintFileName = destFile;
            printerSettings.PrinterName = &quot;Microsoft Print to PDF&quot;;

            if (printerSettings.IsValid)
            {
                SheetRender sr = new SheetRender(wb.Worksheets[wb.Worksheets.ActiveSheetIndex], imgOpt);
                sr.ToPrinter(printerSettings, &quot;test CELLSNET-50063 and CELLSNET-50088&quot;);

                //wait max 1s
                int count = 0;
                while (count &lt; 10 &amp;&amp; !File.Exists(destFile))
                {
                    Thread.Sleep(1000);
                    count++;
                }

                if (count &lt; 10)
                {
                    string content = File.ReadAllText(destFile);
                    //only one page in pdf.
                    Assert.IsTrue(content.IndexOf(&quot;/Count 1&quot;) &gt; -1);
                }
            }
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


