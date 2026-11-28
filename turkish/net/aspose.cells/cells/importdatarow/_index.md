---
title: "Cells.ImportDataRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir DataRow'u Excel dosyasına aktarır"
type: docs
url: /tr/net/aspose.cells/cells/importdatarow/
---
## Cells.ImportDataRow method

Bir DataRow'u Excel dosyasına içe aktarır.

```csharp
public void ImportDataRow(DataRow dataRow, int row, int firstColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dataRow | DataRow | DataRow nesnesi. |
| satır | Int32 | Satır indeksi. |
| firstColumn | Int32 | İlk sütun indeksi. |

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataRowWithDataRowInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Örnek bir DataTable oluştur
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));

            // Örnek veri ekleyin.
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);

            // DataTable'dan ilk satırı çalışma sayfasına, satır 0, sütun 0'dan başlayarak içe aktar
            cells.ImportDataRow(dataTable.Rows[0], 0, 0);

            // Çalışma kitabını kaydedin
            workbook.Save("ImportDataRowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


