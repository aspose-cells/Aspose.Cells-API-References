---
title: PageSetup.IsHFScaleWithDoc
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007
type: docs
url: /net/aspose.cells/pagesetup/ishfscalewithdoc/
---
## PageSetup.IsHFScaleWithDoc property

Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007.

```csharp
public bool IsHFScaleWithDoc { get; set; }
```

### Examples

```csharp
// Called: pageSetup.IsHFScaleWithDoc = true;
public static void Property_IsHFScaleWithDoc()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet in the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the PageSetup object
            PageSetup pageSetup = worksheet.PageSetup;

            // Set the print area
            pageSetup.PrintArea = &quot;D1:K13&quot;;

            // Set the print title columns
            pageSetup.PrintTitleColumns = &quot;$A:$A&quot;;

            // Set the print title rows
            pageSetup.PrintTitleRows = &quot;$1:$1&quot;;

            // Set other page setup properties
            pageSetup.BlackAndWhite = true;
            pageSetup.CenterHorizontally = true;
            pageSetup.CenterVertically = true;
            pageSetup.PrintDraft = false;
            pageSetup.FooterMargin = 1.0; // in centimeters
            pageSetup.FooterMarginInch = 0.39; // in inches
            pageSetup.HeaderMargin = 1.0; // in centimeters
            pageSetup.HeaderMarginInch = 0.39; // in inches
            pageSetup.LeftMargin = 1.0; // in centimeters
            pageSetup.LeftMarginInch = 0.39; // in inches
            pageSetup.RightMargin = 1.0; // in centimeters
            pageSetup.RightMarginInch = 0.39; // in inches
            pageSetup.TopMargin = 1.0; // in centimeters
            pageSetup.TopMarginInch = 0.39; // in inches
            pageSetup.BottomMargin = 1.0; // in centimeters
            pageSetup.BottomMarginInch = 0.39; // in inches
            pageSetup.FirstPageNumber = 1;
            pageSetup.FitToPagesTall = 1;
            pageSetup.FitToPagesWide = 1;
            pageSetup.IsPercentScale = false;
            pageSetup.Order = PrintOrderType.OverThenDown;
            pageSetup.PaperSize = PaperSizeType.PaperA4;
            pageSetup.Orientation = PageOrientationType.Portrait;
            pageSetup.PrintComments = PrintCommentsType.PrintNoComments;
            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDisplayed;
            pageSetup.PrintHeadings = true;
            pageSetup.PrintGridlines = true;
            pageSetup.Zoom = 100;
            pageSetup.IsAutoFirstPageNumber = true;
            pageSetup.PrintQuality = 600;
            pageSetup.PrintCopies = 1;
            pageSetup.IsHFDiffOddEven = false;
            pageSetup.IsHFDiffFirst = false;
            pageSetup.IsHFScaleWithDoc = true;
            pageSetup.IsHFAlignMargins = true;

            // Save the workbook
            workbook.Save(&quot;PageSetupExample.xlsx&quot;);
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


