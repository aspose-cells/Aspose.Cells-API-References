---
title: PageSetup.BlackAndWhite
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents if elements of the document will be printed in black and white
type: docs
url: /net/aspose.cells/pagesetup/blackandwhite/
---
## PageSetup.BlackAndWhite property

Represents if elements of the document will be printed in black and white.

```csharp
public bool BlackAndWhite { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(pageSetup1.BlackAndWhite, pageSetup2.BlackAndWhite, "!" + sheetName + "--PageSetup's BlackAndWhite");
private static void PageSetup_Property_BlackAndWhite(
            String sheetName, PageSetup pageSetup1, PageSetup pageSetup2)
        {
            Assert.AreEqual(pageSetup1.FirstPageNumber, pageSetup2.FirstPageNumber, "!" + sheetName + "--PageSetup's firstPageNumber");
            Assert.AreEqual(pageSetup1.FitToPagesTall, pageSetup2.FitToPagesTall, "!" + sheetName + "--PageSetup's FitToPagesTall");
            Assert.AreEqual(pageSetup1.FitToPagesWide, pageSetup2.FitToPagesWide, "!" + sheetName + "--PageSetup's FitToPagesWide");
            Assert.AreEqual(pageSetup1.CenterHorizontally, pageSetup2.CenterHorizontally, "!" + sheetName + "--PageSetup's CenterHorizontally");
            Assert.AreEqual(pageSetup1.CenterVertically, pageSetup2.CenterVertically, "!" + sheetName + "--PageSetup's CenterVertically");
            Assert.AreEqual(pageSetup1.BlackAndWhite, pageSetup2.BlackAndWhite, "!" + sheetName + "--PageSetup's BlackAndWhite");            
            Assert.AreEqual(pageSetup1.PrintHeadings, pageSetup2.PrintHeadings, "!" + sheetName + "--PageSetup's PrintHeadings");            
            Assert.AreEqual(pageSetup1.PrintGridlines, pageSetup2.PrintGridlines, "!" + sheetName + "--PageSetup's PrintGridlines");            
            Assert.AreEqual(pageSetup1.Orientation, pageSetup2.Orientation, "!" + sheetName + "--PageSetup's Orientation");
            Assert.AreEqual(pageSetup1.PrintQuality, pageSetup2.PrintQuality, "!" + sheetName + "--PageSetup's getPrintQuality");
            Assert.AreEqual(pageSetup1.Order, pageSetup2.Order, "!" + sheetName + "--PageSetup's Order");
           // Assert.AreEqual(pageSetup1.PaperSize, pageSetup2.PaperSize, "!" + sheetName + "--PageSetup's PaperSize");
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


