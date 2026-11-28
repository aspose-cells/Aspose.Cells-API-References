---
title: "SqlScriptColumnTypeMap.GetStringType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SqlScriptColumnTypeMap yöntemi. Veritabanında string tipini alır"
type: docs
url: /tr/net/aspose.cells.saving/sqlscriptcolumntypemap/getstringtype/
---
## SqlScriptColumnTypeMap.GetStringType method

Veritabanındaki metin türünü alır.

```csharp
public virtual string GetStringType()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptColumnTypeMapMethodGetStringTypeDemo
    {
        public static void Run()
        {
            // SqlScriptColumnTypeMap sınıfının bir örneğini oluşturun
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // Varsayılan string tipini al ve görüntüle
            string stringType = columnTypeMap.GetStringType();
            Console.WriteLine("Default String Type: " + stringType);

            // String veri içeren basit bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John Doe");

            // Tip haritasını kullanarak SQL betik seçenekleriyle kaydet
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };
            
            workbook.Save("SqlScriptOutput.sql", saveOptions);
            Console.WriteLine("SQL script saved with string type: " + stringType);
        }
    }
}
```

### Ayrıca Bakınız

* class [SqlScriptColumnTypeMap](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


