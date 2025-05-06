---
title: ImageOrPrintOptions.AllColumnsInOnePagePerSheet
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. If AllColumnsInOnePagePerSheet is true  all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid and the other settings of pagesetup will still take effect
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/
---
## ImageOrPrintOptions.AllColumnsInOnePagePerSheet property

If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

```csharp
public bool AllColumnsInOnePagePerSheet { get; set; }
```

### Examples

```csharp
// Called: pngOptions.ImageOrPrintOptions.AllColumnsInOnePagePerSheet = true;
[Test]
        public void Property_AllColumnsInOnePagePerSheet()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells[&quot;A1&quot;].PutValue(&quot;sdfsdf&quot;);
            Aspose.Cells.ImageSaveOptions pngOptions = new Aspose.Cells.ImageSaveOptions();
            pngOptions.ImageOrPrintOptions.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            pngOptions.ImageOrPrintOptions.AllColumnsInOnePagePerSheet = true;
            pngOptions.ImageOrPrintOptions.OnePagePerSheet = true;
            MemoryStream ms = new MemoryStream();
            workbook.Save(ms, pngOptions);
            byte x = ms.GetBuffer()[0];
            Assert.AreEqual(0x89, x);
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


