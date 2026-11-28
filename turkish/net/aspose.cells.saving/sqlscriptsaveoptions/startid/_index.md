---
title: "SqlScriptSaveOptions.StartId"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SqlScriptSaveOptions özelliği. Başlangıç kimliğini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.saving/sqlscriptsaveoptions/startid/
---
## SqlScriptSaveOptions.StartId property

Başlangıç kimliğini alır ve ayarlar.

```csharp
public int StartId { get; set; }
```

### Açıklamalar

Yalnızca [`IdName`](../idname/) ayarlandığında çalışır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyStartIdDemo
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

            // StartId'i 100 olarak ayarlayarak SQL dışa aktarma seçeneklerini yapılandır
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                IdName = "ID",
                StartId = 100, // Demonstrating StartId property
                HasHeaderRow = true,
                OperatorType = SqlScriptOperatorType.Insert
            };

            // SQL betiği olarak kaydet
            workbook.Save("Employees_WithStartId.sql", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


