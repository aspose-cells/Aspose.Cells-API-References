---
title: "ImportTableOptions.IsHtmlString"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImportTableOptions özelliği. Değerin html etiketleri içerip içermediğini gösterir."
type: docs
url: /tr/net/aspose.cells/importtableoptions/ishtmlstring/
---
## ImportTableOptions.IsHtmlString property

Değerin html etiketleri içerip içermediğini gösterir.

```csharp
public bool IsHtmlString { get; set; }
```

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyIsHtmlStringDemo
    {
        public static void Run()
        {
            // HTML içeren örnek verilerle bir DataTable oluştur.
            DataTable table = new DataTable();
            table.Columns.Add("ID");
            table.Columns.Add("Content");
            table.Columns.Add("Time");
            
            // HTML içeriğiyle bir satır ekle.
            table.Rows.Add("1", "<a href='https://www.example.com'>Example Link</a>", "2:30 PM");

            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // IsHtmlString true olarak ayarlanmış DataTable'ı içe aktar.
            worksheet.Cells.ImportData(table, 0, 0, new ImportTableOptions
            {
                IsFieldNameShown = true,
                IsHtmlString = true,
                NumberFormats = new string[] { null, null, "h:mm AM/PM" }
            });

            // Çalışma kitabını kaydedin
            workbook.Save("HtmlStringImportDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


