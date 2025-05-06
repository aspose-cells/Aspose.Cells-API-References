---
title: PdfBookmarkEntry.Destination
second_title: Aspose.Cells for .NET API Reference
description: PdfBookmarkEntry property. The cell to which the bookmark link
type: docs
url: /net/aspose.cells.rendering/pdfbookmarkentry/destination/
---
## PdfBookmarkEntry.Destination property

The cell to which the bookmark link.

```csharp
public Cell Destination { get; set; }
```

### Examples

```csharp
// Called: subPbe3.Destination = cellInPage4;
[Test, Description(&quot;PdfSaveOptions.Bookmark property need be checked by Manual&quot;)]
        public void Property_Destination()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();
            Cell cellInPage1 = workbook.Worksheets[0].Cells[0, 0];
            Cell cellInPage2 = workbook.Worksheets[1].Cells[0, 0];
            Cell cellInPage3 = workbook.Worksheets[2].Cells[0, 0];
            Cell cellInPage4 = workbook.Worksheets[3].Cells[0, 0];
            Cell cellInPage5 = workbook.Worksheets[4].Cells[0, 0];
            cellInPage1.PutValue(&quot;page1&quot;);
            cellInPage2.PutValue(&quot;page2&quot;);
            cellInPage3.PutValue(&quot;page3&quot;);
            cellInPage4.PutValue(&quot;page4&quot;);
            cellInPage5.PutValue(&quot;page5&quot;);

            PdfBookmarkEntry pbeRoot = new PdfBookmarkEntry();
            pbeRoot.Text = &quot;root&quot;;
            pbeRoot.Destination = cellInPage1;
            pbeRoot.SubEntry = new System.Collections.ArrayList();
            pbeRoot.IsOpen = false;

            PdfBookmarkEntry subPbe1 = new PdfBookmarkEntry();
            subPbe1.Text = &quot;section1&quot;;
            subPbe1.Destination = cellInPage2;

            PdfBookmarkEntry subPbe2 = new PdfBookmarkEntry();
            subPbe2.Text = &quot;section2&quot;;
            subPbe2.Destination = cellInPage3;

            PdfBookmarkEntry subPbe3 = new PdfBookmarkEntry();
            subPbe3.Text = &quot;section3&quot;;
            subPbe3.Destination = cellInPage4;

            PdfBookmarkEntry subPbe4 = new PdfBookmarkEntry();
            subPbe4.Text = &quot;section4&quot;;
            subPbe4.Destination = cellInPage5;

            pbeRoot.SubEntry.Add(subPbe1);
            pbeRoot.SubEntry.Add(subPbe2);
            pbeRoot.SubEntry.Add(subPbe3);
            pbeRoot.SubEntry.Add(subPbe4);

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.Bookmark = pbeRoot;
            workbook.Save(Constants.checkPath + &quot;PdfSaveOptions_Bookmark_003.pdf&quot;, pdfSaveOptions);
        }
```

### See Also

* class [Cell](../../../aspose.cells/cell/)
* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


