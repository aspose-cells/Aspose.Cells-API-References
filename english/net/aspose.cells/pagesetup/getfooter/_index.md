---
title: PageSetup.GetFooter
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Gets a script formatting the footer of an Excel file
type: docs
url: /net/aspose.cells/pagesetup/getfooter/
---
## PageSetup.GetFooter method

Gets a script formatting the footer of an Excel file.

```csharp
public string GetFooter(int section)
```

| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |

### Examples

```csharp
// Called: Assert.AreEqual(pagesetup.GetFooter(2), null);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;pagesetup\\pagesetup1.xls&quot;);
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pagesetup = worksheet.PageSetup;
            ReflectInvoker.invoke(&quot;pagesetup&quot;, pagesetup, new Object[][]{
                //Page
                new Object[]{&quot;Orientation&quot;, PageOrientationType.Landscape},
                new Object[] {&quot;FitToPagesWide&quot;, 1},
                new Object[] {&quot;FitToPagesTall&quot;, 2},
                new Object[] {&quot;PaperSize&quot;, PaperSizeType.PaperA4},
                new Object[] {&quot;PrintQuality&quot;, 120},
                new Object[] {&quot;FirstPageNumber&quot;, 1},
                //Margins
                new Object[] {&quot;TopMargin&quot;, 2.5, 0.01},
               new Object[] {&quot;LeftMargin&quot;, 1.9, 0.1},
                new Object[] {&quot;RightMargin&quot;, 1.9, 0.1},
                new Object[] {&quot;BottomMargin&quot;, 2.5, 0.01},
                new Object[] {&quot;HeaderMargin&quot;, 1.3, 0.01},
                new Object[] {&quot;FooterMargin&quot;, 1.3, 0.01},
                new Object[] {&quot;CenterHorizontally&quot;, false},
                new Object[] {&quot;CenterVertically&quot;, false},
                ////Header/Footer
                //new Object[] {&quot;GetHeader(0)&quot;, &quot;&quot;},
                //new Object[] {&quot;GetHeader(1)&quot;, &quot;01/05/2007 DDI,�й�,Econometrics    Team H&quot;},
                //new Object[] {&quot;GetHeader(2)&quot;, &quot;&quot;},
                //new Object[] {&quot;GetFooter(0)&quot;, &quot;&quot;},
                //new Object[] {&quot;GetFooter(1)&quot;, &quot;Trivision--Year 1&quot;},
                //new Object[] {&quot;GetFooter(2)&quot;, &quot;&quot;},
                //Sheet
                new Object[] {&quot;PrintArea&quot;, &quot;A1:I41&quot;},
                //new Object[] {&quot;PrintTitleRows&quot;, &quot;&quot;},
                //new Object[] {&quot;PrintTitleColumns&quot;, &quot;&quot;},
                new Object[] {&quot;PrintGridlines&quot;, false},
                new Object[] {&quot;BlackAndWhite&quot;, false},
                new Object[] { &quot;PrintDraft&quot;, false},
                new Object[] {&quot;PrintHeadings&quot;, false},
                new Object[] {&quot;PrintComments&quot;, PrintCommentsType.PrintNoComments},
                new Object[] {&quot;PrintErrors&quot;, PrintErrorsType.PrintErrorsDisplayed},
                new Object[] {&quot;Order&quot;, PrintOrderType.DownThenOver}
             });

            //Header/Footer
            Assert.AreEqual(pagesetup.GetHeader(0), null);
            Assert.AreEqual(pagesetup.GetHeader(1), &quot;&amp;\&quot;Arial,加粗\&quot;01/05/2007 DDI,&amp;\&quot;宋体,加粗\&quot;中国&amp;\&quot;Arial,加粗\&quot;,Econometrics    Team H&quot;);
            Assert.AreEqual(pagesetup.GetHeader(2), null);
            Assert.AreEqual(pagesetup.GetFooter(0), null);
            Assert.AreEqual(pagesetup.GetFooter(1), &quot;&amp;\&quot;Arial,Bold\&quot;Trivision--Year 1&quot;);
            Assert.AreEqual(pagesetup.GetFooter(2), null);
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


