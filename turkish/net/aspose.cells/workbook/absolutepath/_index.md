---
title: "Workbook.AbsolutePath"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Dosyanın mutlak yolunu alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/workbook/absolutepath/
---
## Workbook.AbsolutePath property

Dosyanın mutlak yolunu alır ve ayarlar.

```csharp
public string AbsolutePath { get; set; }
```

### Açıklamalar

Yalnızca dış bağlantılar için kullanılır.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyAbsolutePathDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook sourceBook = new Workbook();
            
            // Bazı çalışma sayfaları ekle
            sourceBook.Worksheets.Add("Sheet1");
            sourceBook.Worksheets.Add("Sheet2");

            // Fiziksel bir yol elde etmek için çalışma kitabını kaydedin
            string sourcePath = Path.GetFullPath("output");
            if (!Directory.Exists(sourcePath))
            {
                Directory.CreateDirectory(sourcePath);
            }
            string sourceFilePath = Path.Combine(sourcePath, "example.xlsx");
            sourceBook.Save(sourceFilePath);

            // AbsolutePath özelliğini göstermek için çalışma kitabını yeniden açın
            Workbook reopenedBook = new Workbook(sourceFilePath);
            
            // Tam yolu oluşturmak için AbsolutePath özelliğini kullanın
            string pathToBook = Path.Combine(reopenedBook.AbsolutePath, reopenedBook.FileName);
            Console.WriteLine("Full path to workbook: " + pathToBook);

            // Yolu kullanarak köprüler ekleyin
            SetHyperlink(reopenedBook.Worksheets[0], 0, pathToBook, reopenedBook.Worksheets[0].Name, "A1");
            SetHyperlink(reopenedBook.Worksheets[0], 1, pathToBook, reopenedBook.Worksheets[1].Name, "B1");

            // Değiştirilmiş çalışma kitabını kaydet
            string destPath = Path.Combine(sourcePath, "modified_example.xlsx");
            reopenedBook.Save(destPath);
        }

        private static void SetHyperlink(Worksheet sheet, int linkIndex, string path, string sheetName, string cellRef)
        {
            HyperlinkCollection hyperlinks = sheet.Hyperlinks;
            hyperlinks.Add(cellRef, 1, 1, path + "#" + sheetName + "!A1");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


