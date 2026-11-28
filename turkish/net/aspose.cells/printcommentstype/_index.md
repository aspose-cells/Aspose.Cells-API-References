---
title: "Enum PrintCommentsType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.PrintCommentsType enum. Yorumların sayfa ile nasıl yazdırıldığını temsil eder"
type: docs
url: /tr/net/aspose.cells/printcommentstype/
---
## PrintCommentsType enumeration

Yorumların sayfa ile birlikte nasıl yazdırılacağını temsil eder.

```csharp
public enum PrintCommentsType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| PrintInPlace | `0` | Sayfada görüntülendiği gibi yorumları yazdırmayı temsil eder. |
| PrintNoComments | `1` | Yorumları yazdırmamayı temsil eder. |
| PrintSheetEnd | `2` | Yorumları sayfanın sonunda yazdırmayı temsil eder. |
| PrintWithThreadedComments | `3` | Sayfada görüntülendiği gibi yorumları, iş parçacıklı yorumları da içerecek şekilde yazdırmayı temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintCommentsTypeDemo
    {
        public static void PrintCommentsTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı yorumlar ekleyin
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a comment.";

            commentIndex = worksheet.Comments.Add("B2");
            comment = worksheet.Comments[commentIndex];
            comment.Note = "This is another comment.";

            // Sayfa ayarlarında yorum yazdırma türünü ayarlayın
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.PrintComments = PrintCommentsType.PrintSheetEnd;

            // Çalışma kitabını bir dosyaya kaydedin
            workbook.Save("PrintCommentsTypeExample.xlsx");

            Console.WriteLine("Workbook saved successfully with comments printed at the end of the sheet.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


