---
title: "ImportTableOptions.TotalRows"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImportTableOptions özelliği. Veri kaynağından içe aktarılacak toplam satır sayısını alır veya ayarlar. 1, verilen veri kaynağının tüm satırları anlamına gelir"
type: docs
url: /tr/net/aspose.cells/importtableoptions/totalrows/
---
## ImportTableOptions.TotalRows property

Veri kaynağından içe aktarılacak toplam satır sayısını alır veya ayarlar. -1, verilen veri kaynağının tüm satırları anlamına gelir.

```csharp
public int TotalRows { get; set; }
```

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyTotalRowsDemo
    {
        public static void Run()
        {
            // Örnek bir DataTable oluştur
            DataTable table = new DataTable("TestTable");
            table.Columns.Add("Column1", typeof(string));
            table.Columns.Add("Column2", typeof(int));
            
            // Örnek veri ekleyin.
            table.Rows.Add("Item1", 100);
            table.Rows.Add("Item2", 200);
            table.Rows.Add("Item3", 300);

            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // TotalRows özelliği 2 olarak ayarlanmış ImportTableOptions oluşturun (sadece ilk 2 satırı içe aktarır)
            ImportTableOptions options = new ImportTableOptions
            {
                IsFieldNameShown = true,
                TotalRows = 2 // Only import 2 rows from the DataTable
            };

            // Belirtilen seçeneklerle verileri içe aktar
            worksheet.Cells.ImportData(table, 0, 0, options);

            // Çalışma kitabını kaydedin
            workbook.Save("ImportWithTotalRows.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Data imported with TotalRows=2. Only first 2 rows were imported.");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


