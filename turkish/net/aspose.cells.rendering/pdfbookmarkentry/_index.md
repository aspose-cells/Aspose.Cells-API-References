---
title: "Sınıf PdfBookmarkEntry"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.PdfBookmarkEntry sınıfı. PdfBookmarkEntry, pdf yer imlerinde bir giriştir. Eğer mevcut örneğin Text özelliği null ise veya mevcut örnek gizlenecek ve çocuklar mevcut seviyeye eklenecektir."
type: docs
url: /tr/net/aspose.cells.rendering/pdfbookmarkentry/
---
## PdfBookmarkEntry class

PdfBookmarkEntry, pdf yer işaretinde bir giriştir. Eğer geçerli örneğin Text özelliği null veya \"\" ise, geçerli örnek gizlenecek ve alt öğeler mevcut seviyeye eklenecektir.

```csharp
public class PdfBookmarkEntry
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PdfBookmarkEntry](pdfbookmarkentry/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Destination](../../aspose.cells.rendering/pdfbookmarkentry/destination/) { get; set; } | Yer imi bağlantısının yönlendirildiği hücre. |
| [DestinationName](../../aspose.cells.rendering/pdfbookmarkentry/destinationname/) { get; set; } | Hedefin adını alır veya ayarlar. |
| [IsCollapse](../../aspose.cells.rendering/pdfbookmarkentry/iscollapse/) { get; set; } | Bu özellik true olduğunda, bookmarkentry daralır, aksi takdirde genişler. |
| [IsOpen](../../aspose.cells.rendering/pdfbookmarkentry/isopen/) { get; set; } | Bu özellik true olduğunda, bookmarkentry genişler, aksi takdirde daralır. |
| [SubEntry](../../aspose.cells.rendering/pdfbookmarkentry/subentry/) { get; set; } | Bir yer iminin alt girişi. |
| [Text](../../aspose.cells.rendering/pdfbookmarkentry/text/) { get; set; } | Bir yer iminin başlığı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Collections;

    public class PdfBookmarkEntryDemo
    {
        public static void PdfBookmarkEntryExample()
        {
            // Yeni bir çalışma kitabı oluşturun ve çalışma sayfaları ekleyin
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();

            // Her çalışma sayfasından hücreleri alın
            Cell cellInPage1 = workbook.Worksheets[0].Cells["A1"];
            Cell cellInPage2 = workbook.Worksheets[1].Cells["A1"];
            Cell cellInPage3 = workbook.Worksheets[2].Cells["A1"];

            // Hücrelere değerler koyun
            cellInPage1.PutValue("page1");
            cellInPage2.PutValue("page2");
            cellInPage3.PutValue("page3");

            // Kök PdfBookmarkEntry oluşturun
            PdfBookmarkEntry pbeRoot = new PdfBookmarkEntry
            {
                Text = "root",  // if pbeRoot.Text = null, all children of pbeRoot will be inserted on the top level in the bookmark.
                Destination = cellInPage1,
                SubEntry = new ArrayList(),
                IsOpen = false
            };

            // Alt PdfBookmarkEntry'ler oluşturun
            PdfBookmarkEntry subPbe1 = new PdfBookmarkEntry
            {
                Text = "section1",
                Destination = cellInPage2
            };

            PdfBookmarkEntry subPbe2 = new PdfBookmarkEntry
            {
                Text = "section2",
                Destination = cellInPage3
            };

            // Alt girişleri kök girişe ekleyin
            pbeRoot.SubEntry.Add(subPbe1);
            pbeRoot.SubEntry.Add(subPbe2);

            // PdfSaveOptions oluşturun ve yer imini ayarlayın
            PdfSaveOptions saveOptions = new PdfSaveOptions
            {
                Bookmark = pbeRoot
            };

            // Çalışma kitabını yer imleriyle PDF olarak kaydedin
            workbook.Save("output_bookmark.pdf", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


