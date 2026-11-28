---
title: "PageSetup.PrintComments"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Yorumların sayfa ile birlikte nasıl yazdırılacağını temsil eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/printcomments/
---
## PageSetup.PrintComments property

Yorumların sayfa ile birlikte nasıl yazdırılacağını temsil eder.

```csharp
public PrintCommentsType PrintComments { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintCommentsDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // A1 hücresine bir yorum ekle
            int commentIndex = sheet.Comments.Add("A1");
            Comment comment = sheet.Comments[commentIndex];
            comment.Note = "This is a test comment";

            // Farklı yazdırma yorum seçeneklerini ayarlayın ve etkilerini gösterin
            sheet.PageSetup.PrintComments = PrintCommentsType.PrintInPlace;
            Console.WriteLine("PrintComments set to PrintInPlace");

            sheet.PageSetup.PrintComments = PrintCommentsType.PrintSheetEnd;
            Console.WriteLine("PrintComments set to PrintSheetEnd");

            sheet.PageSetup.PrintComments = PrintCommentsType.PrintNoComments;
            Console.WriteLine("PrintComments set to PrintNoComments");

            // Ayarların kalıcı olduğunu göstermek için çalışma kitabını kaydedin
            workbook.Save("PrintCommentsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* enum [PrintCommentsType](../../printcommentstype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


