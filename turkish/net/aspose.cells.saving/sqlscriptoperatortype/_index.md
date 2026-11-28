---
title: "Enum SqlScriptOperatorType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Saving.SqlScriptOperatorType enum. İşletme verisinin türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.saving/sqlscriptoperatortype/
---
## SqlScriptOperatorType enumeration

İşletme verisinin türünü temsil eder.

```csharp
public enum SqlScriptOperatorType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Insert | `0` | Veri ekle. |
| Update | `1` | Veriyi güncelle. |
| Delete | `2` | Veriyi sil. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SqlScriptOperatorTypeDemo
    {
        public static void SqlScriptOperatorTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);

            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue("Charlie");

            // SqlScriptSaveOptions oluştur ve özellikleri ayarla
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                CheckIfTableExists = true,
                AddBlankLineBetweenRows = true,
                Separator = ';',
                OperatorType = SqlScriptOperatorType.Insert,
                PrimaryKey = 0,
                CreateTable = true,
                IdName = "ID",
                StartId = 1,
                TableName = "SampleTable",
                ExportAsString = false,
                ExportArea = new CellArea { StartRow = 1, StartColumn = 0, EndRow = 3, EndColumn = 1 },
                HasHeaderRow = true
            };

            // Çalışma kitabını SQL betiği olarak kaydet
            workbook.Save("SqlScriptOperatorTypeExample.sql", saveOptions);

            // Sonuçları çıktı olarak ver.
            Console.WriteLine("SQL script has been saved successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


