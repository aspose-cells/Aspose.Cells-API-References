---
title: "Cells.ImportDataView"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir DataView'i çalışma sayfasına içe aktarır"
type: docs
url: /tr/net/aspose.cells/cells/importdataview/
---
## Cells.ImportDataView method

Bir DataView'i çalışma sayfasına içe aktarır.

```csharp
public int ImportDataView(DataView dataView, int firstRow, int firstColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dataView | DataView | İçe aktarılacak DataView nesnesi. |
| firstRow | Int32 | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | İçe aktarılacak ilk hücrenin sütun numarası. |

### Dönüş Değeri

Aktarılan toplam satır sayısı

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataViewWithDataViewInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Örnek DataTable oluştur
            DataTable table = new DataTable("Products");
            table.Columns.Add("ID", typeof(int));
            table.Columns.Add("Name", typeof(string));
            table.Columns.Add("Price", typeof(decimal));

            // Örnek veri ekleyin.
            table.Rows.Add(1, "Laptop", 999.99m);
            table.Rows.Add(2, "Smartphone", 699.99m);
            table.Rows.Add(3, "Tablet", 399.99m);

            // DataTable'dan DataView oluştur
            DataView dataView = new DataView(table);

            // DataView'i satır 0, sütun 0'dan başlayan çalışma sayfasına içe aktar
            cells.ImportDataView(dataView, 0, 0);

            // Çalışma kitabını kaydedin
            workbook.Save("ImportDataViewOutput.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


