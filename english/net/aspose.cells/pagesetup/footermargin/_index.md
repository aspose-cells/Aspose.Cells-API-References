---
title: PageSetup.FooterMargin
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the distance from the bottom of the page to the footer in unit of centimeters
type: docs
url: /net/aspose.cells/pagesetup/footermargin/
---
## PageSetup.FooterMargin property

Represents the distance from the bottom of the page to the footer, in unit of centimeters.

```csharp
public double FooterMargin { get; set; }
```

### Examples

```csharp
// Called: pageSetup.FooterMargin = 1.0; // in centimeters
public static void PageSetup_Property_FooterMargin()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet in the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the PageSetup object
            PageSetup pageSetup = worksheet.PageSetup;

            // Set the print area
            pageSetup.PrintArea = "D1:K13";

            // Set the print title columns
            pageSetup.PrintTitleColumns = "$A:$A";

            // Set the print title rows
            pageSetup.PrintTitleRows = "$1:$1";

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
            workbook.Save("PageSetupExample.xlsx");
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


