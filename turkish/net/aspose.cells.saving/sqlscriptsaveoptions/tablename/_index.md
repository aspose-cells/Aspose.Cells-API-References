---
title: "SqlScriptSaveOptions.TableName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SqlScriptSaveOptions özelliği. Tablo adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.saving/sqlscriptsaveoptions/tablename/
---
## SqlScriptSaveOptions.TableName property

Tablo adını alır ve ayarlar.

```csharp
public string TableName { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyTableNameDemo
    {
        public static void Run()
        {
            // Bazı verilerle örnek bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Özel tablo adıyla SQL kaydetme seçeneklerini yapılandırın
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions();
            saveOptions.TableName = "Employees"; // Demonstrating TableName property
            saveOptions.CreateTable = true;
            saveOptions.OperatorType = SqlScriptOperatorType.Insert;

            // SQL betiği olarak kaydet
            workbook.Save("output.sql", saveOptions);

            Console.WriteLine("SQL Script generated with table name 'Employees'");
        }
    }
}
```

### Ayrıca Bakınız

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


