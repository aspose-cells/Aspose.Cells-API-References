---
title: "ImportTableOptions.ConvertGridStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImportTableOptions özelliği. Izgara görünümünün hücrelere uygulanıp uygulanmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/importtableoptions/convertgridstyle/
---
## ImportTableOptions.ConvertGridStyle property

Izgara görünümünün stilinin hücrelere uygulanıp uygulanmayacağını belirtir.

```csharp
public bool ConvertGridStyle { get; set; }
```

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyConvertGridStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri oluştur
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            dataTable.Rows.Add(101, "Laptop", 999.99m);
            dataTable.Rows.Add(102, "Monitor", 249.50m);

            // ConvertGridStyle etkinleştirilmiş şekilde içe aktarma seçeneklerini ayarla
            ImportTableOptions options = new ImportTableOptions();
            options.ConvertGridStyle = true; // This will apply grid styling to the imported data
            options.IsFieldNameShown = true;

            // Stil ile veri içe aktar
            worksheet.Cells.ImportData(dataTable, 0, 0, options);

            // Sonucu kaydet
            workbook.Save("ImportWithGridStyle.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


