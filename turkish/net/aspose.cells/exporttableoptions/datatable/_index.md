---
title: "ExportTableOptions.DataTable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExportTableOptions özelliği. Sütun veri tipinin atandığı DataTable'ı alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/exporttableoptions/datatable/
---
## ExportTableOptions.DataTable property

Sütunların veri tipi atanan DataTable'ı alır ve ayarlar.

```csharp
public DataTable DataTable { get; set; }
```

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyDataTableDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Hücrelere örnek veri ekle
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue(100);
            cells["B2"].PutValue("Text1");
            cells["A3"].PutValue(200);
            cells["B3"].PutValue("Text2");

            // DataTable oluştur ve sütunları tanımla
            DataTable dt = new DataTable();
            dt.Columns.Add("NumericData", typeof(double));
            dt.Columns.Add("TextData", typeof(string));

            // Dışa aktarma seçeneklerini yapılandır
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true;
            options.Indexes = new int[] { 0, 1 }; // Export both columns
            options.DataTable = dt;

            // Verileri DataTable'a dışa aktar
            cells.ExportDataTable(0, 0, 3, 2, options);

            // Dışa aktarılan veriyi göster
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row["NumericData"]}, {row["TextData"]}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


