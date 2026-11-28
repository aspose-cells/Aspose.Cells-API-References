---
title: "ExportTableOptions.ExportColumnName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExportTableOptions özelliği. İlk satırdaki verilerin DataTable'ın sütun adına aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells/exporttableoptions/exportcolumnname/
---
## ExportTableOptions.ExportColumnName property

İlk satırdaki verilerin DataTable'ın sütun adı olarak dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

```csharp
public bool ExportColumnName { get; set; }
```

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyExportColumnNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Çalışma sayfasında örnek veri oluştur
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue(100);
            cells["B2"].PutValue("Data1");
            cells["A3"].PutValue(200);
            cells["B3"].PutValue("Data2");

            // Dışa aktarma seçeneklerini yapılandır
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true; // Demonstrating ExportColumnName property
            options.IsVertical = true;
            options.Indexes = new int[] { 0, 1 }; // Export all columns

            // Çalışma sayfasındaki verileri DataTable'a dışa aktar
            DataTable dataTable = cells.ExportDataTable(0, 0, 4, 2, options);

            // Dışa aktarılan veriyi göster
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row["Column1"]}, {row["Column2"]}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


