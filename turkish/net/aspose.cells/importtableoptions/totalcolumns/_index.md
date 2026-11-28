---
title: "ImportTableOptions.TotalColumns"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImportTableOptions özelliği. Veri kaynağından içe aktarılacak toplam sütun sayısını alır veya ayarlar. 1, verilen veri kaynağının tüm satırları anlamına gelir"
type: docs
url: /tr/net/aspose.cells/importtableoptions/totalcolumns/
---
## ImportTableOptions.TotalColumns property

Veri kaynağından içe aktarılacak toplam sütun sayısını alır veya ayarlar. -1, verilen veri kaynağının tüm satırları anlamına gelir.

```csharp
public int TotalColumns { get; set; }
```

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyTotalColumnsDemo
    {
        public static void Run()
        {
            // Örnek bir DataTable oluştur
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            // Örnek veri ekleyin.
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);

            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // TotalColumns = 2 ile içe aktarma seçeneklerini ayarla (sadece ilk 2 sütunu içe aktarır)
            ImportTableOptions importOptions = new ImportTableOptions
            {
                IsFieldNameShown = true,
                TotalColumns = 2 // Only import first 2 columns (ID and Name)
            };

            // Veriyi A1 hücresinden başlayarak içe aktar
            cells.ImportData(dataTable, 0, 0, importOptions);

            // Çalışma kitabını kaydedin
            workbook.Save("ImportWithTotalColumns.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Data imported with TotalColumns=2. Only first 2 columns were imported.");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


