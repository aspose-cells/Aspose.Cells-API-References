---
title: "MarkdownSaveOptions.TableHeaderType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MarkdownSaveOptions özelliği. Tablo başlığının nasıl ayarlandığını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/markdownsaveoptions/tableheadertype/
---
## MarkdownSaveOptions.TableHeaderType property

Tablo başlığının nasıl ayarlandığını alır ve ayarlar.

```csharp
public MarkdownTableHeaderType TableHeaderType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markdown;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsPropertyTableHeaderTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir tablo oluşturmak için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // MarkdownSaveOptions oluştur ve TableHeaderType'ı ayarla
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;

            // Belirtilen seçeneklerle markdown olarak kaydet
            workbook.Save("output.md", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* enum [MarkdownTableHeaderType](../../../aspose.cells.markdown/markdowntableheadertype/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


