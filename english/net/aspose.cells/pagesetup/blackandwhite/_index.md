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
// Called: Assert.AreEqual(pageSetup1.BlackAndWhite, pageSetup2.BlackAndWhite, &amp;quot;!&amp;quot; + sheetName + &amp;quot;--PageSetup&amp;apos;s BlackAndWhite&amp;quot;);
private static void Property_BlackAndWhite(
            String sheetName, PageSetup pageSetup1, PageSetup pageSetup2)
        {
            Assert.AreEqual(pageSetup1.FirstPageNumber, pageSetup2.FirstPageNumber, &quot;!&quot; + sheetName + &quot;--PageSetup&apos;s firstPageNumber&quot;);
            Assert.AreEqual(pageSetup1.FitToPagesTall, pageSetup2.FitToPagesTall, &quot;!&quot; + sheetName + &quot;--PageSetup&apos;s FitToPagesTall&quot;);
            Assert.AreEqual(pageSetup1.FitToPagesWide, pageSetup2.FitToPagesWide, &quot;!&quot; + sheetName + &quot;--PageSetup&apos;s FitToPagesWide&quot;);
            Assert.AreEqual(pageSetup1.CenterHorizontally, pageSetup2.CenterHorizontally, &quot;!&quot; + sheetName + &quot;--PageSetup&apos;s CenterHorizontally&quot;);
            Assert.AreEqual(pageSetup1.CenterVertically, pageSetup2.CenterVertically, &quot;!&quot; + sheetName + &quot;--PageSetup&apos;s CenterVertically&quot;);
            Assert.AreEqual(pageSetup1.BlackAndWhite, pageSetup2.BlackAndWhite, &quot;!&quot; + sheetName + &quot;--PageSetup&apos;s BlackAndWhite&quot;);            
            Assert.AreEqual(pageSetup1.PrintHeadings, pageSetup2.PrintHeadings, &quot;!&quot; + sheetName + &quot;--PageSetup&apos;s PrintHeadings&quot;);            
            Assert.AreEqual(pageSetup1.PrintGridlines, pageSetup2.PrintGridlines, &quot;!&quot; + sheetName + &quot;--PageSetup&apos;s PrintGridlines&quot;);            
            Assert.AreEqual(pageSetup1.Orientation, pageSetup2.Orientation, &quot;!&quot; + sheetName + &quot;--PageSetup&apos;s Orientation&quot;);
            Assert.AreEqual(pageSetup1.PrintQuality, pageSetup2.PrintQuality, &quot;!&quot; + sheetName + &quot;--PageSetup&apos;s getPrintQuality&quot;);
            Assert.AreEqual(pageSetup1.Order, pageSetup2.Order, &quot;!&quot; + sheetName + &quot;--PageSetup&apos;s Order&quot;);
           // Assert.AreEqual(pageSetup1.PaperSize, pageSetup2.PaperSize, &quot;!&quot; + sheetName + &quot;--PageSetup&apos;s PaperSize&quot;);
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


