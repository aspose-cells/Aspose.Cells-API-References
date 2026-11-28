---
title: "ImportTableOptions.InsertRows"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImportTableOptions özelliği. Yeni satırların veri kayıtlarını içe aktarmak için eklenip eklenmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/importtableoptions/insertrows/
---
## ImportTableOptions.InsertRows property

Veri kayıtlarını içe aktarmak için yeni satırların eklenip eklenmeyeceğini gösterir.

```csharp
public bool InsertRows { get; set; }
```

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyInsertRowsDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Örnek veri tablosu oluştur
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            dataTable.Rows.Add(1, "Laptop", 999.99);
            dataTable.Rows.Add(2, "Monitor", 249.99);
            dataTable.Rows.Add(3, "Keyboard", 49.99);

            // Mevcut veriyi çalışma sayfasına ekleyin (ekleme ile aşağı kaydırılacak)
            cells["A1"].PutValue("Existing Data");
            cells["A2"].PutValue(100);

            // InsertRows = true ile içe aktarma seçeneklerini ayarlayın
            ImportTableOptions options = new ImportTableOptions();
            options.InsertRows = true; // This will insert new rows instead of overwriting
            options.IsFieldNameShown = true;

            // Satır 1'den başlayarak verileri içe aktar (mevcut verinin altına satırlar eklenecek)
            cells.ImportData(dataTable, 1, 0, options);

            // Çalışma kitabını kaydedin
            workbook.Save("InsertRowsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


