---
title: "SqlScriptSaveOptions.CreateTable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SqlScriptSaveOptions özelliği. Tablo oluşturma SQL'inin dışa aktarılıp aktarılmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells.saving/sqlscriptsaveoptions/createtable/
---
## SqlScriptSaveOptions.CreateTable property

Tablo oluşturma SQL'ini dışa aktarmayı belirtir.

```csharp
public bool CreateTable { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyCreateTableDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // CreateTable etkinleştirilmiş şekilde SQL dışa aktarma seçeneklerini yapılandır
            SqlScriptSaveOptions options = new SqlScriptSaveOptions
            {
                CreateTable = true,
                TableName = "Employees",
                HasHeaderRow = true
            };

            // SQL betiği olarak kaydet
            workbook.Save("output.sql", options);
        }
    }
}
```

### Ayrıca Bakınız

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


