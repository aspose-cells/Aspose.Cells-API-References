---
title: "Worksheet.RefreshPivotTables"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Bu Worksheet'teki tüm PivotTable'ları yeniler"
type: docs
url: /tr/net/aspose.cells/worksheet/refreshpivottables/
---
## RefreshPivotTables() {#refreshpivottables_1}

Bu çalışma sayfasındaki tüm PivotTable'ları yeniler.

```csharp
public void RefreshPivotTables()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRefreshPivotTablesDemo
    {
        public static void Run()
        {
            // Pivot tabloları içeren kaynak Excel dosyasından bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook("example.xlsx");
            
            // Pivot tablolarını içeren ilk çalışma sayfasını alın
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasındaki tüm pivot tabloları yenileyin
            worksheet.RefreshPivotTables();
            
            // Güncellenmiş çalışma kitabını kaydedin
            workbook.Save("RefreshedPivotTables.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshPivotTables(PivotTableRefreshOption) {#refreshpivottables}

Bu çalışma sayfasındaki tüm PivotTable'ları yeniler.

```csharp
public bool RefreshPivotTables(PivotTableRefreshOption option)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| seçenek | PivotTableRefreshOption | Pivot tablo veri kaynağını yenilemek için seçenek. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class WorksheetMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;

            // Bir pivot tablo oluştur
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            worksheet.RefreshPivotTables();

            int preCount = pivotTable.RowFields[0].PivotItems.Count;


            // Kaynak veriyi değiştir
            worksheet.Cells["A2"].Value = "test2";
            worksheet.Cells["A3"].Value = "test3";

            // Yenileme seçenekleri oluştur
            PivotTableRefreshOption options = new PivotTableRefreshOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All // Fixed: Changed ReserveAll to All
            };
            worksheet.RefreshPivotTables(options);
            int nowCount = pivotTable.RowFields[0].PivotItems.Count;
            Console.WriteLine(nowCount > preCount);
                        

            // Sonucu kaydet
            workbook.Save("WorksheetMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTableRefreshOption](../../../aspose.cells.pivot/pivottablerefreshoption/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


