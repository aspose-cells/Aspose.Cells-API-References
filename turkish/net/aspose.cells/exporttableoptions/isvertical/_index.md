---
title: "ExportTableOptions.IsVertical"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExportTableOptions özelliği. Workbook dosyasındaki bir satır DataTable'daki bir satırı temsil ediyorsa true, bir sütun DataTable'daki bir satırı temsil ediyorsa false"
type: docs
url: /tr/net/aspose.cells/exporttableoptions/isvertical/
---
## ExportTableOptions.IsVertical property

Workbook dosyasındaki bir satır DataTable'da bir satırı temsil ediyorsa true. Workbook dosyasındaki bir sütun DataTable'da bir satırı temsil ediyorsa false.

```csharp
public bool IsVertical { get; set; }
```

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyIsVerticalDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Çalışma sayfasında örnek veri oluştur
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(25);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(30);

            // DataTable oluştur
            DataTable dt = new DataTable();
            dt.Columns.Add("Column1", typeof(string));
            dt.Columns.Add("Column2", typeof(int));

            // IsVertical = true ile ExportTableOptions ayarla
            ExportTableOptions options = new ExportTableOptions();
            options.IsVertical = true;
            options.ExportColumnName = true;
            options.DataTable = dt;

            // Verileri dikey olarak dışa aktar
            cells.ExportDataTable(0, 0, 2, 2, options);

            // Dışa aktarılan DataTable'ı göster
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row[0]}, {row[1]}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


