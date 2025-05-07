---
title: SheetRender.PageCount
second_title: Aspose.Cells for .NET API Reference
description: SheetRender property. Gets the total page count of current worksheet
type: docs
url: /net/aspose.cells.rendering/sheetrender/pagecount/
---
## SheetRender.PageCount property

Gets the total page count of current worksheet.

```csharp
public int PageCount { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1, sr.PageCount);
[Test]
        public void Property_PageCount()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CELLSJAVA-42356.xlsx");

            ImageOrPrintOptions imgOpts = new ImageOrPrintOptions();
            imgOpts.ImageType = ImageType.Png;
            imgOpts.OnePagePerSheet = true;
            imgOpts.OutputBlankPageWhenNothingToPrint = true;

            SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpts);
            Assert.AreEqual(1, sr.PageCount);
            
            MemoryStream ms = new MemoryStream();
            sr.ToImage(0, ms);
            Assert.IsTrue(ms.ToArray().Length > 0);
        }
```

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


