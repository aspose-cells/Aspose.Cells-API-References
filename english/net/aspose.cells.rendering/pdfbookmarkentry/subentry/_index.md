---
title: PdfBookmarkEntry.SubEntry
second_title: Aspose.Cells for .NET API Reference
description: PdfBookmarkEntry property. SubEntry of a bookmark
type: docs
url: /net/aspose.cells.rendering/pdfbookmarkentry/subentry/
---
## PdfBookmarkEntry.SubEntry property

SubEntry of a bookmark.

```csharp
public ArrayList SubEntry { get; set; }
```

### Examples

```csharp
// Called: pbeRoot.SubEntry.Add(subPbe1);
[Test, Description("PdfSaveOptions.Bookmark property need be checked by Manual")]
        public void Property_SubEntry()
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
            cellInPage1.PutValue("page1");
            cellInPage2.PutValue("page2");
            cellInPage3.PutValue("page3");
            cellInPage4.PutValue("page4");
            cellInPage5.PutValue("page5");

            PdfBookmarkEntry pbeRoot = new PdfBookmarkEntry();
            pbeRoot.Text = "root";
            pbeRoot.Destination = cellInPage1;
            pbeRoot.SubEntry = new System.Collections.ArrayList();
            pbeRoot.IsOpen = false;

            PdfBookmarkEntry subPbe1 = new PdfBookmarkEntry();
            subPbe1.Text = "section1";
            subPbe1.Destination = cellInPage2;

            PdfBookmarkEntry subPbe2 = new PdfBookmarkEntry();
            subPbe2.Text = "section2";
            subPbe2.Destination = cellInPage3;

            PdfBookmarkEntry subPbe3 = new PdfBookmarkEntry();
            subPbe3.Text = "section3";
            subPbe3.Destination = cellInPage4;

            PdfBookmarkEntry subPbe4 = new PdfBookmarkEntry();
            subPbe4.Text = "section4";
            subPbe4.Destination = cellInPage5;

            pbeRoot.SubEntry.Add(subPbe1);
            pbeRoot.SubEntry.Add(subPbe2);
            pbeRoot.SubEntry.Add(subPbe3);
            pbeRoot.SubEntry.Add(subPbe4);

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.Bookmark = pbeRoot;
            workbook.Save(Constants.checkPath + "PdfSaveOptions_Bookmark_003.pdf", pdfSaveOptions);
        }
```

### See Also

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


