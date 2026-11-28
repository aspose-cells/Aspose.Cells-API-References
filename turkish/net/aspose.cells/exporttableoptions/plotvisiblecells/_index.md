---
title: "ExportTableOptions.PlotVisibleCells"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExportTableOptions özelliği. Yalnızca görünen hücreleri dışa aktarır"
type: docs
url: /tr/net/aspose.cells/exporttableoptions/plotvisiblecells/
---
## ExportTableOptions.PlotVisibleCells property

Yalnızca görünen hücreleri dışa aktarır.

```csharp
public bool PlotVisibleCells { get; set; }
```

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyPlotVisibleCellsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Gizli satır/sütunları olan örnek veri ekle
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["C1"].PutValue("Header3");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue("Data3");
            
            // Satır 2'yi ve B sütununu (indeks 1) gizle
            worksheet.Cells.HideRow(1);
            worksheet.Cells.HideColumn(1);

            // PlotVisibleCells true olarak ayarlanmış dışa aktarma seçenekleri oluştur
            ExportTableOptions exportOptions = new ExportTableOptions
            {
                PlotVisibleCells = true,
                PlotVisibleColumns = true,
                PlotVisibleRows = true
            };

            // Yalnızca görünen hücreleri dışa aktar
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 3, exportOptions);

            // Dışa aktarılan veriyi göster (yalnızca görünen hücreler dışa aktarılmalı)
            Console.WriteLine("Exported Data:");
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


