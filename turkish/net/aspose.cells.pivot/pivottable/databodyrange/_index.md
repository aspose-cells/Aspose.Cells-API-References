---
title: "PivotTable.DataBodyRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Başlık satırı ile ekleme satırı arasındaki listede veri alanını içeren aralığı temsil eden bir CellArea nesnesi döndürür. Salt okunur"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/databodyrange/
---
## PivotTable.DataBodyRange property

Başlık satırı ile ekleme satırı arasındaki listede veri alanını içeren aralığı temsil eden bir [`CellArea`](../../../aspose.cells/cellarea/) nesnesi döndürür. Salt okunur.

```csharp
public CellArea DataBodyRange { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataBodyRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Özet tablo için örnek veri ekle
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bike";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Car";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bike";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Car";
            cells["B5"].Value = 2500;

            // Pivot tablo ekle
            int pivotIndex = sheet.PivotTables.Add("A7", "A1:B5", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            // Pivot tabloyu yapılandır
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Özet tablo verilerini yenile
            pivot.RefreshData();
            pivot.CalculateData();

            // DataBodyRange kullanımını göster
            CellArea dataBodyArea = pivot.DataBodyRange;
            Console.WriteLine($"Data body range: StartRow={dataBodyArea.StartRow}, EndRow={dataBodyArea.EndRow}, StartColumn={dataBodyArea.StartColumn}, EndColumn={dataBodyArea.EndColumn}");

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableDataBodyRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


