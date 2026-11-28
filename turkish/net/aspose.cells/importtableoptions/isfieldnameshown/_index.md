---
title: "ImportTableOptions.IsFieldNameShown"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImportTableOptions özelliği. Alan adının içe aktarılıp aktarılmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/importtableoptions/isfieldnameshown/
---
## ImportTableOptions.IsFieldNameShown property

Alan adının içe aktarılıp aktarılmayacağını gösterir.

```csharp
public bool IsFieldNameShown { get; set; }
```

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyIsFieldNameShownDemo
    {
        public static void Run()
        {
            // Örnek bir DataTable oluştur
            DataTable table = new DataTable();
            table.Columns.Add("ID");
            table.Columns.Add("Product");
            
            // Örnek veri ekleyin.
            table.Rows.Add(1, "Laptop");
            table.Rows.Add(2, "Smartphone");
            table.Rows.Add(3, "Tablet");

            // Bir çalışma kitabı oluştur ve alan adları gösterilerek veriyi içe aktar
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;  // Show field names
            options.InsertRows = true;       // Insert new rows
            
            // Veriyi 5. satır, 0. sütundan başlayarak içe aktar
            cells.ImportData(table, 5, 0, options);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ImportDataWithFieldNames.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


