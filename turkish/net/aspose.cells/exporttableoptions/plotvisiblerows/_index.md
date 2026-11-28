---
title: "ExportTableOptions.PlotVisibleRows"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExportTableOptions özelliği. Yalnızca görünen satırları dışa aktarır"
type: docs
url: /tr/net/aspose.cells/exporttableoptions/plotvisiblerows/
---
## ExportTableOptions.PlotVisibleRows property

Yalnızca görünen satırları dışa aktarır.

```csharp
public bool PlotVisibleRows { get; set; }
```

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyPlotVisibleRowsDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur ve ilk çalışma sayfasına eriş
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Çalışma sayfasında örnek veri oluştur
            cells["A1"].PutValue("Column1");
            cells["A2"].PutValue(10);
            cells["A3"].PutValue(20);
            cells["A4"].PutValue(30);

            // 20 değerini içeren satır 3'ü (indeks 2) gizle
            worksheet.Cells.HideRow(2);

            // Dışa aktarılacak bir DataTable oluştur
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Column1", typeof(int));

            // Dışa aktarma seçeneklerini ayarla
            ExportTableOptions options = new ExportTableOptions();
            options.PlotVisibleRows = true; // Only export visible rows
            options.ExportColumnName = true;
            options.DataTable = dataTable;

            // Veriyi dışa aktar (gizli satırı atlamalı)
            cells.ExportDataTable(0, 0, 4, 1, options);

            // Dışa aktarılan verileri görüntüle
            Console.WriteLine("Exported Data (PlotVisibleRows=true):");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine(row["Column1"]);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


