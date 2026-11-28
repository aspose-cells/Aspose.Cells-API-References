---
title: "ImportTableOptions.ColumnIndexes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImportTableOptions özelliği. Veri kaynağından içe aktarılacak sütunları 0 tabanlı olarak alır veya ayarlar. null, tüm sütunların içe aktarılması gerektiği anlamına gelir."
type: docs
url: /tr/net/aspose.cells/importtableoptions/columnindexes/
---
## ImportTableOptions.ColumnIndexes property

Veri kaynağından içe aktarılacak sütunları (0 tabanlı) alır veya ayarlar. null, tüm sütunların içe aktarılması gerektiği anlamına gelir.

```csharp
public int[] ColumnIndexes { get; set; }
```

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyColumnIndexesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek DataTable oluştur
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            // Örnek veri ekleyin.
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);
            dataTable.Rows.Add(3, "Product C", 39.99m);

            // İçe aktarma seçeneklerini yalnızca 0 ve 2 indekslerindeki sütunları (ID ve Fiyat) içe aktaracak şekilde ayarlayın.
            ImportTableOptions options = new ImportTableOptions();
            options.ColumnIndexes = new int[] { 0, 2 };
            options.IsFieldNameShown = true;

            // Belirtilen sütun indeksleriyle verileri içe aktar.
            worksheet.Cells.ImportData(dataTable, 0, 0, options);

            // Çalışma kitabını kaydedin
            workbook.Save("ColumnIndexesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


