---
title: "SqlScriptSaveOptions.CheckAllDataForColumnType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SqlScriptSaveOptions özelliği. Tüm verileri kontrol ederek sütunların veri tipini bulur"
type: docs
url: /tr/net/aspose.cells.saving/sqlscriptsaveoptions/checkalldataforcolumntype/
---
## SqlScriptSaveOptions.CheckAllDataForColumnType property

Sütunların veri tipini bulmak için tüm verileri kontrol edin.

```csharp
public bool CheckAllDataForColumnType { get; set; }
```

### Açıklamalar

Varsayılan değer false'tur, performans için yalnızca ilk satırı kontrol ederiz. Bu özellik true ise ve sütunlar karışık değer tipleri içeriyorsa, sütunların tipi metin olacaktır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyCheckAllDataForColumnTypeDemo
    {
        public static void Run()
        {
            // Test verileriyle örnek bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Karışık tiplerde örnek veri ekle
            sheet.Cells["A1"].PutValue("First_name");
            sheet.Cells["B1"].PutValue("Last_name");
            sheet.Cells["C1"].PutValue("age");
            sheet.Cells["D1"].PutValue("tax");
            
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["B2"].PutValue("Doe");
            sheet.Cells["C2"].PutValue(30);
            sheet.Cells["D2"].PutValue("10%");
            
            sheet.Cells["A3"].PutValue("Jane");
            sheet.Cells["B3"].PutValue("Smith");
            sheet.Cells["C3"].PutValue(25);
            sheet.Cells["D3"].PutValue(0.15);

            // SQL kaydetme seçeneklerini yapılandır
            SqlScriptSaveOptions sqlSaveOptions = new SqlScriptSaveOptions();
            sqlSaveOptions.OperatorType = SqlScriptOperatorType.Insert;
            sqlSaveOptions.CreateTable = true;
            sqlSaveOptions.CheckAllDataForColumnType = true; // This will examine all data to determine column types
            
            // SQL betiği olarak kaydet - Save yöntemi string döndürmez, bu yüzden önce kaydetmemiz ve ardından dosyayı okumanız gerekir
            wb.Save("output.sql", sqlSaveOptions);
            
            // Oluşturulan SQL betiğini okuyun
            string sqlScript = System.IO.File.ReadAllText("output.sql");
            
            Console.WriteLine("SQL Script generated:");
            Console.WriteLine(sqlScript);
        }
    }
}
```

### Ayrıca Bakınız

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


