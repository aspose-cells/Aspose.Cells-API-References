---
title: "Font.Charset"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Font özelliği. Karakter kümesini temsil eder"
type: docs
url: /tr/net/aspose.cells/font/charset/
---
## Font.Charset property

Karakter kümesini temsil eder.

```csharp
public int Charset { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyCharsetDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Karakter kümesi dahil belirli yazı tipi özelliklerine sahip bir stil oluştur
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.Charset = 1; // ANSI_CHARSET

            // Stili bir hücreye uygula
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Text with ANSI charset");

            // Farklı karakter kümesiyle başka bir stil oluştur
            Style style2 = workbook.CreateStyle();
            style2.Font.Name = "Times New Roman";
            style2.Font.Size = 12;
            style2.Font.Charset = 2; // DEFAULT_CHARSET

            // İkinci stili başka bir hücreye uygula
            Cell cell2 = worksheet.Cells["A2"];
            cell2.SetStyle(style2);
            cell2.PutValue("Text with DEFAULT charset");

            // Çalışma kitabını kaydedin
            workbook.Save("FontCharsetDemo.xlsx");

            // Karakter kümesi özelliklerini doğrula
            Console.WriteLine("Cell A1 Font Charset: " + cell.GetStyle().Font.Charset);
            Console.WriteLine("Cell A2 Font Charset: " + cell2.GetStyle().Font.Charset);
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


