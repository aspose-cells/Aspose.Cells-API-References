---
title: "SqlScriptSaveOptions.SheetIndexes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SqlScriptSaveOptions özelliği. Dışa aktarılan sayfaların indekslerini temsil eder"
type: docs
url: /tr/net/aspose.cells.saving/sqlscriptsaveoptions/sheetindexes/
---
## SqlScriptSaveOptions.SheetIndexes property

Dışa aktarılan sayfaların indekslerini temsil eder.

```csharp
public int[] SheetIndexes { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SqlScriptSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // Birden çok sayfa içeren yeni bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Tüm sayfalara bazı veriler ekleyin
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet worksheet = workbook.Worksheets[i];
                worksheet.Cells["A1"].PutValue("ID");
                worksheet.Cells["B1"].PutValue("Name");
                worksheet.Cells["A2"].PutValue(1);
                worksheet.Cells["B2"].PutValue("John");
                worksheet.Cells["A3"].PutValue(2);
                worksheet.Cells["B3"].PutValue("Jane");
            }

            // SqlScriptSaveOptions örneği oluştur
            SqlScriptSaveOptions options = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                CreateTable = true,
                HasHeaderRow = true
            };

            // Mevcut SheetIndexes değerini göster (null tüm sayfalar anlamına gelir)
            Console.WriteLine("Initial SheetIndexes: " + 
                (options.SheetIndexes == null ? "All sheets" : string.Join(",", options.SheetIndexes)));

            // SheetIndexes'i sadece birinci ve üçüncü sayfaları (0 ve 2) dışa aktarmak için ayarla
            options.SheetIndexes = new int[] { 0, 2 };

            // Seçeneklerle kaydet
            workbook.Save("SqlScriptExportSelectedSheets.sql", options);

            // SheetIndexes'i sadece ikinci sayfayı dışa aktarmak için değiştir
            options.SheetIndexes = new int[] { 1 };
            workbook.Save("SqlScriptExportSecondSheet.sql", options);

            // Tüm sayfaları dışa aktarmak için SheetIndexes'i null olarak ayarlayın
            options.SheetIndexes = null;
            workbook.Save("SqlScriptExportAllSheets.sql", options);
        }
    }
}
```

### Ayrıca Bakınız

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


