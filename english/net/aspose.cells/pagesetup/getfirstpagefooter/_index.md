---
title: PageSetup.GetFirstPageFooter
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Gets a script formatting the first page footer of an Excel file
type: docs
url: /net/aspose.cells/pagesetup/getfirstpagefooter/
---
## PageSetup.GetFirstPageFooter method

Gets a script formatting the first page footer of an Excel file.

```csharp
public string GetFirstPageFooter(int section)
```

| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |

### Examples

```csharp
// Called: AssertHelper.AreEqual(pagesetupSrc.GetFirstPageFooter(0), pagesetupDest.GetFirstPageFooter(0), info + &amp;quot;.GetFirstPageFooter(0)&amp;quot;);
public static void Method_Int32_(PageSetup pagesetupSrc, PageSetup pagesetupDest, string info)
        {
            if (AssertHelper.checkNull(pagesetupSrc, pagesetupDest, info))
            {
                return;
            }
            //==============properties are supported in excel 2003 format file====================//
            //Page
            AssertHelper.AreEqual(pagesetupSrc.Orientation, pagesetupDest.Orientation, info + &quot;.Orientation&quot;);
            AssertHelper.AreEqual(pagesetupSrc.IsPercentScale, pagesetupDest.IsPercentScale, info + &quot;.IsPercentScale&quot;);
            AssertHelper.AreEqual(pagesetupSrc.Zoom, pagesetupDest.Zoom, info + &quot;.Zoom&quot;);            
            AssertHelper.AreEqual(pagesetupSrc.FitToPagesWide, pagesetupDest.FitToPagesWide, info + &quot;.FitToPagesWide&quot;);
            AssertHelper.AreEqual(pagesetupSrc.FitToPagesTall, pagesetupDest.FitToPagesTall, info + &quot;.FitToPagesTall&quot;);
            AssertHelper.AreEqual(pagesetupSrc.PaperSize, pagesetupDest.PaperSize, info + &quot;.PaperSize&quot;);
            AssertHelper.AreEqual(pagesetupSrc.PrintQuality, pagesetupDest.PrintQuality, info + &quot;.PrintQuality&quot;);
            AssertHelper.AreEqual(pagesetupSrc.FirstPageNumber, pagesetupDest.FirstPageNumber, info + &quot;.FirstPageNumber&quot;);
            //Margins
            AssertHelper.AreEqual(pagesetupSrc.TopMargin, pagesetupDest.TopMargin, delta, info + &quot;.TopMargin&quot;);
            AssertHelper.AreEqual(pagesetupSrc.LeftMargin, pagesetupDest.LeftMargin, delta, info + &quot;.LeftMargin&quot;);
            AssertHelper.AreEqual(pagesetupSrc.RightMargin, pagesetupDest.RightMargin, delta, info + &quot;.RightMargin&quot;);
            AssertHelper.AreEqual(pagesetupSrc.BottomMargin, pagesetupDest.BottomMargin, delta, info + &quot;.BottomMargin&quot;);
            AssertHelper.AreEqual(pagesetupSrc.HeaderMargin, pagesetupDest.HeaderMargin, delta, info + &quot;.HeaderMargin&quot;);
            AssertHelper.AreEqual(pagesetupSrc.FooterMargin, pagesetupDest.FooterMargin, delta, info + &quot;.FooterMargin&quot;);
            AssertHelper.AreEqual(pagesetupSrc.CenterHorizontally, pagesetupDest.CenterHorizontally, info + &quot;.CenterHorizontally&quot;);
            AssertHelper.AreEqual(pagesetupSrc.CenterVertically, pagesetupDest.CenterVertically, info + &quot;.CenterVertically&quot;);
            //Header/Footer
            AssertHelper.AreEqual(pagesetupSrc.GetHeader(0), pagesetupDest.GetHeader(0), info + &quot;.GetHeader(0)&quot;);
            AssertHelper.AreEqual(pagesetupSrc.GetHeader(1), pagesetupDest.GetHeader(1), info + &quot;.GetHeader(1)&quot;);
            AssertHelper.AreEqual(pagesetupSrc.GetHeader(2), pagesetupDest.GetHeader(2), info + &quot;.GetHeader(2)&quot;);
            AssertHelper.AreEqual(pagesetupSrc.GetFooter(0), pagesetupDest.GetFooter(0), info + &quot;.GetFooter(0)&quot;);
            AssertHelper.AreEqual(pagesetupSrc.GetFooter(1), pagesetupDest.GetFooter(1), info + &quot;.GetFooter(1)&quot;);
            AssertHelper.AreEqual(pagesetupSrc.GetFooter(2), pagesetupDest.GetFooter(2), info + &quot;.GetFooter(2)&quot;);
         
            
            //Sheet
            AssertHelper.AreEqual(pagesetupSrc.PrintArea, pagesetupDest.PrintArea, info + &quot;.PrintArea&quot;);
            AssertHelper.AreEqual(pagesetupSrc.PrintTitleRows, pagesetupDest.PrintTitleRows, info + &quot;.PrintTitleRows&quot;);
            AssertHelper.AreEqual(pagesetupSrc.PrintTitleColumns, pagesetupDest.PrintTitleColumns, info + &quot;.PrintTitleColumns&quot;);
            AssertHelper.AreEqual(pagesetupSrc.PrintGridlines, pagesetupDest.PrintGridlines, info + &quot;.PrintGridlines&quot;);
            AssertHelper.AreEqual(pagesetupSrc.BlackAndWhite, pagesetupDest.BlackAndWhite, info + &quot;.BlackAndWhite&quot;);
            AssertHelper.AreEqual(pagesetupSrc.PrintDraft, pagesetupDest.PrintDraft, info + &quot;.PrintDraft&quot;);
            AssertHelper.AreEqual(pagesetupSrc.PrintHeadings, pagesetupDest.PrintHeadings, info + &quot;.PrintHeadings&quot;);
            AssertHelper.AreEqual(pagesetupSrc.PrintComments, pagesetupDest.PrintComments, info + &quot;.PrintComments&quot;);
            AssertHelper.AreEqual(pagesetupSrc.PrintErrors, pagesetupDest.PrintErrors, info + &quot;.PrintErrors&quot;);
            AssertHelper.AreEqual(pagesetupSrc.Order, pagesetupDest.Order, info + &quot;.Order&quot;);

            //==============properties are supported in excel 2007 format file====================//
            //Header/Footer
            AssertHelper.AreEqual(pagesetupSrc.IsHFDiffOddEven, pagesetupDest.IsHFDiffOddEven, info + &quot;.IsHFDiffOddEven&quot;);
            if (pagesetupSrc.IsHFDiffOddEven)
            {
                AssertHelper.AreEqual(pagesetupSrc.GetEvenHeader(0), pagesetupDest.GetEvenHeader(0), info + &quot;.GetEvenHeader(0)&quot;);
                AssertHelper.AreEqual(pagesetupSrc.GetEvenHeader(1), pagesetupDest.GetEvenHeader(1), info + &quot;.GetEvenHeader(1)&quot;);
                AssertHelper.AreEqual(pagesetupSrc.GetEvenHeader(2), pagesetupDest.GetEvenHeader(2), info + &quot;.GetEvenHeader(2)&quot;);
                AssertHelper.AreEqual(pagesetupSrc.GetEvenFooter(0), pagesetupDest.GetEvenFooter(0), info + &quot;.GetEvenFooter(0)&quot;);
                AssertHelper.AreEqual(pagesetupSrc.GetEvenFooter(1), pagesetupDest.GetEvenFooter(1), info + &quot;.GetEvenFooter(1)&quot;);
                AssertHelper.AreEqual(pagesetupSrc.GetEvenFooter(2), pagesetupDest.GetEvenFooter(2), info + &quot;.GetEvenFooter(2)&quot;);
            }
            AssertHelper.AreEqual(pagesetupSrc.IsHFDiffFirst, pagesetupDest.IsHFDiffFirst, info + &quot;.IsHFDiffFirst&quot;);
            if (pagesetupSrc.IsHFDiffFirst)
            {
                AssertHelper.AreEqual(pagesetupSrc.GetFirstPageHeader(0), pagesetupDest.GetFirstPageHeader(0), info + &quot;.GetFirstPageHeader(0)&quot;);
                AssertHelper.AreEqual(pagesetupSrc.GetFirstPageHeader(1), pagesetupDest.GetFirstPageHeader(1), info + &quot;.GetFirstPageHeader(1)&quot;);
                AssertHelper.AreEqual(pagesetupSrc.GetFirstPageHeader(2), pagesetupDest.GetFirstPageHeader(2), info + &quot;.GetFirstPageHeader(2)&quot;);
                AssertHelper.AreEqual(pagesetupSrc.GetFirstPageFooter(0), pagesetupDest.GetFirstPageFooter(0), info + &quot;.GetFirstPageFooter(0)&quot;);
                AssertHelper.AreEqual(pagesetupSrc.GetFirstPageFooter(1), pagesetupDest.GetFirstPageFooter(1), info + &quot;.GetFirstPageFooter(1)&quot;);
                AssertHelper.AreEqual(pagesetupSrc.GetFirstPageFooter(2), pagesetupDest.GetFirstPageFooter(2), info + &quot;.GetFirstPageFooter(2)&quot;);
            }
            AssertHelper.AreEqual(pagesetupSrc.IsHFScaleWithDoc, pagesetupDest.IsHFScaleWithDoc, info + &quot;.IsHFScaleWithDoc&quot;);
            AssertHelper.AreEqual(pagesetupSrc.IsHFAlignMargins, pagesetupDest.IsHFAlignMargins, info + &quot;.IsHFAlignMargins&quot;);
          
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


