---
title: "Sınıf SqlScriptColumnTypeMap"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Saving.SqlScriptColumnTypeMap sınıfı. Sütun tür haritasını temsil eder"
type: docs
url: /tr/net/aspose.cells.saving/sqlscriptcolumntypemap/
---
## SqlScriptColumnTypeMap class

Sütun türü haritasını temsil eder.

```csharp
public class SqlScriptColumnTypeMap
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [SqlScriptColumnTypeMap](sqlscriptcolumntypemap/)() | Varsayılan yapıcı. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| virtual [GetNumbericType](../../aspose.cells.saving/sqlscriptcolumntypemap/getnumberictype/)() | (**Obsolete.**) Veritabanındaki sayısal türü alır. |
| virtual [GetNumberType](../../aspose.cells.saving/sqlscriptcolumntypemap/getnumbertype/)() | Veritabanındaki sayısal türü alır. |
| virtual [GetStringType](../../aspose.cells.saving/sqlscriptcolumntypemap/getstringtype/)() | Veritabanındaki metin türünü alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SqlScriptColumnTypeMapDemo
    {
        public static void SqlScriptColumnTypeMapExample()
        {
            // SqlScriptColumnTypeMap sınıfının bir örneğini oluşturun
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // GetStringType ve GetNumbericType yöntemlerinin kullanımını gösterin
            string stringType = columnTypeMap.GetStringType();
            string numericType = columnTypeMap.GetNumbericType();

            // Sonuçları konsola yazdırın
            Console.WriteLine("String Type in Database: " + stringType);
            Console.WriteLine("Numeric Type in Database: " + numericType);

            // SqlScriptSaveOptions bir örnek oluşturun ve ColumnTypeMap'i ayarlayın
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };

            // Bir çalışma kitabı oluşturun ve bazı veriler ekleyin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John Doe");

            // Çalışma kitabını kaydetme seçeneklerini kullanarak SQL betiği olarak kaydedin
            workbook.Save("SqlScriptExample.sql", saveOptions);

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


