---
title: PageSetup.PrintDraft
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents if the sheet will be printed without graphics
type: docs
url: /net/aspose.cells/pagesetup/printdraft/
---
## PageSetup.PrintDraft property

Represents if the sheet will be printed without graphics.

```csharp
public bool PrintDraft { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(pagesetupSrc.PrintDraft, pagesetupDest.PrintDraft, info + ".PrintDraft");
public static void Property_PrintDraft(PageSetup pagesetupSrc, PageSetup pagesetupDest, string info)
        {
            if (AssertHelper.checkNull(pagesetupSrc, pagesetupDest, info))
            {
                return;
            }
            //==============properties are supported in excel 2003 format file====================//
            //Page
            AssertHelper.AreEqual(pagesetupSrc.Orientation, pagesetupDest.Orientation, info + ".Orientation");
            AssertHelper.AreEqual(pagesetupSrc.IsPercentScale, pagesetupDest.IsPercentScale, info + ".IsPercentScale");
            AssertHelper.AreEqual(pagesetupSrc.Zoom, pagesetupDest.Zoom, info + ".Zoom");            
            AssertHelper.AreEqual(pagesetupSrc.FitToPagesWide, pagesetupDest.FitToPagesWide, info + ".FitToPagesWide");
            AssertHelper.AreEqual(pagesetupSrc.FitToPagesTall, pagesetupDest.FitToPagesTall, info + ".FitToPagesTall");
            AssertHelper.AreEqual(pagesetupSrc.PaperSize, pagesetupDest.PaperSize, info + ".PaperSize");
            AssertHelper.AreEqual(pagesetupSrc.PrintQuality, pagesetupDest.PrintQuality, info + ".PrintQuality");
            AssertHelper.AreEqual(pagesetupSrc.FirstPageNumber, pagesetupDest.FirstPageNumber, info + ".FirstPageNumber");
            //Margins
            AssertHelper.AreEqual(pagesetupSrc.TopMargin, pagesetupDest.TopMargin, delta, info + ".TopMargin");
            AssertHelper.AreEqual(pagesetupSrc.LeftMargin, pagesetupDest.LeftMargin, delta, info + ".LeftMargin");
            AssertHelper.AreEqual(pagesetupSrc.RightMargin, pagesetupDest.RightMargin, delta, info + ".RightMargin");
            AssertHelper.AreEqual(pagesetupSrc.BottomMargin, pagesetupDest.BottomMargin, delta, info + ".BottomMargin");
            AssertHelper.AreEqual(pagesetupSrc.HeaderMargin, pagesetupDest.HeaderMargin, delta, info + ".HeaderMargin");
            AssertHelper.AreEqual(pagesetupSrc.FooterMargin, pagesetupDest.FooterMargin, delta, info + ".FooterMargin");
            AssertHelper.AreEqual(pagesetupSrc.CenterHorizontally, pagesetupDest.CenterHorizontally, info + ".CenterHorizontally");
            AssertHelper.AreEqual(pagesetupSrc.CenterVertically, pagesetupDest.CenterVertically, info + ".CenterVertically");
            //Header/Footer
            AssertHelper.AreEqual(pagesetupSrc.GetHeader(0), pagesetupDest.GetHeader(0), info + ".GetHeader(0)");
            AssertHelper.AreEqual(pagesetupSrc.GetHeader(1), pagesetupDest.GetHeader(1), info + ".GetHeader(1)");
            AssertHelper.AreEqual(pagesetupSrc.GetHeader(2), pagesetupDest.GetHeader(2), info + ".GetHeader(2)");
            AssertHelper.AreEqual(pagesetupSrc.GetFooter(0), pagesetupDest.GetFooter(0), info + ".GetFooter(0)");
            AssertHelper.AreEqual(pagesetupSrc.GetFooter(1), pagesetupDest.GetFooter(1), info + ".GetFooter(1)");
            AssertHelper.AreEqual(pagesetupSrc.GetFooter(2), pagesetupDest.GetFooter(2), info + ".GetFooter(2)");
         
            
            //Sheet
            AssertHelper.AreEqual(pagesetupSrc.PrintArea, pagesetupDest.PrintArea, info + ".PrintArea");
            AssertHelper.AreEqual(pagesetupSrc.PrintTitleRows, pagesetupDest.PrintTitleRows, info + ".PrintTitleRows");
            AssertHelper.AreEqual(pagesetupSrc.PrintTitleColumns, pagesetupDest.PrintTitleColumns, info + ".PrintTitleColumns");
            AssertHelper.AreEqual(pagesetupSrc.PrintGridlines, pagesetupDest.PrintGridlines, info + ".PrintGridlines");
            AssertHelper.AreEqual(pagesetupSrc.BlackAndWhite, pagesetupDest.BlackAndWhite, info + ".BlackAndWhite");
            AssertHelper.AreEqual(pagesetupSrc.PrintDraft, pagesetupDest.PrintDraft, info + ".PrintDraft");
            AssertHelper.AreEqual(pagesetupSrc.PrintHeadings, pagesetupDest.PrintHeadings, info + ".PrintHeadings");
            AssertHelper.AreEqual(pagesetupSrc.PrintComments, pagesetupDest.PrintComments, info + ".PrintComments");
            AssertHelper.AreEqual(pagesetupSrc.PrintErrors, pagesetupDest.PrintErrors, info + ".PrintErrors");
            AssertHelper.AreEqual(pagesetupSrc.Order, pagesetupDest.Order, info + ".Order");

            //==============properties are supported in excel 2007 format file====================//
            //Header/Footer
            AssertHelper.AreEqual(pagesetupSrc.IsHFDiffOddEven, pagesetupDest.IsHFDiffOddEven, info + ".IsHFDiffOddEven");
            if (pagesetupSrc.IsHFDiffOddEven)
            {
                AssertHelper.AreEqual(pagesetupSrc.GetEvenHeader(0), pagesetupDest.GetEvenHeader(0), info + ".GetEvenHeader(0)");
                AssertHelper.AreEqual(pagesetupSrc.GetEvenHeader(1), pagesetupDest.GetEvenHeader(1), info + ".GetEvenHeader(1)");
                AssertHelper.AreEqual(pagesetupSrc.GetEvenHeader(2), pagesetupDest.GetEvenHeader(2), info + ".GetEvenHeader(2)");
                AssertHelper.AreEqual(pagesetupSrc.GetEvenFooter(0), pagesetupDest.GetEvenFooter(0), info + ".GetEvenFooter(0)");
                AssertHelper.AreEqual(pagesetupSrc.GetEvenFooter(1), pagesetupDest.GetEvenFooter(1), info + ".GetEvenFooter(1)");
                AssertHelper.AreEqual(pagesetupSrc.GetEvenFooter(2), pagesetupDest.GetEvenFooter(2), info + ".GetEvenFooter(2)");
            }
            AssertHelper.AreEqual(pagesetupSrc.IsHFDiffFirst, pagesetupDest.IsHFDiffFirst, info + ".IsHFDiffFirst");
            if (pagesetupSrc.IsHFDiffFirst)
            {
                AssertHelper.AreEqual(pagesetupSrc.GetFirstPageHeader(0), pagesetupDest.GetFirstPageHeader(0), info + ".GetFirstPageHeader(0)");
                AssertHelper.AreEqual(pagesetupSrc.GetFirstPageHeader(1), pagesetupDest.GetFirstPageHeader(1), info + ".GetFirstPageHeader(1)");
                AssertHelper.AreEqual(pagesetupSrc.GetFirstPageHeader(2), pagesetupDest.GetFirstPageHeader(2), info + ".GetFirstPageHeader(2)");
                AssertHelper.AreEqual(pagesetupSrc.GetFirstPageFooter(0), pagesetupDest.GetFirstPageFooter(0), info + ".GetFirstPageFooter(0)");
                AssertHelper.AreEqual(pagesetupSrc.GetFirstPageFooter(1), pagesetupDest.GetFirstPageFooter(1), info + ".GetFirstPageFooter(1)");
                AssertHelper.AreEqual(pagesetupSrc.GetFirstPageFooter(2), pagesetupDest.GetFirstPageFooter(2), info + ".GetFirstPageFooter(2)");
            }
            AssertHelper.AreEqual(pagesetupSrc.IsHFScaleWithDoc, pagesetupDest.IsHFScaleWithDoc, info + ".IsHFScaleWithDoc");
            AssertHelper.AreEqual(pagesetupSrc.IsHFAlignMargins, pagesetupDest.IsHFAlignMargins, info + ".IsHFAlignMargins");
          
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


