---
title: "MarkdownTableHeaderType enum'ı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Markdown.MarkdownTableHeaderType enum'ı. Markdown dosyasındaki tablonun başlık tipini temsil eder."
type: docs
url: /tr/net/aspose.cells.markdown/markdowntableheadertype/
---
## MarkdownTableHeaderType enumeration

Markdown dosyasındaki tablonun başlık türünü temsil eder.

```csharp
public enum MarkdownTableHeaderType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| FirstRow | `0` | İlk satır tablo başlığı olarak. |
| ColumnHeader | `1` | Sütun adı (A,B,C... gibi) tablo başlığı olarak. |
| Empty | `2` | Boş bir başlık satırı. |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Markdown;

namespace AsposeCellsExamples
{
    public class MarkdownClassMarkdownTableHeaderTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // Markdown kaydetme seçeneklerini ayarla
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;
            
            // Markdown dosyası olarak kaydet
            workbook.Save("output.md", saveOptions);
            
            // Çıktıyı doğrula
            string text = File.ReadAllText("output.md");
            Console.WriteLine(text.Contains("---|") ? "Success" : "Failed");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Markdown](../../aspose.cells.markdown/)
* assembly [Aspose.Cells](../../)


