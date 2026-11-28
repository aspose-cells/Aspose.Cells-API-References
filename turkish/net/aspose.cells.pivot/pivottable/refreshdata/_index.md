---
title: "PivotTable.RefreshData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable yöntemi. Veri kaynağından pivot önbelleğine verileri yeniler"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/refreshdata/
---
## RefreshData() {#refreshdata}

Verileri veri kaynağından pivot önbelleğine yeniler.

```csharp
[Obsolete("Use PivotCache.Refresh() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotRefreshState RefreshData()
```

### Açıklamalar

Veri kaynağından pivot önbelleğine veri toplayacağız, ardından önbellekteki veriyi hücrelere hesaplayacağız. Ve dosyadaki tüm pivot tablolarını tek tek yenilemek yerine sadece [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) yöntemini çağırarak yenileyip hesaplayabilirsiniz. NOT: Bu yöntem artık kullanımdan kaldırıldı. Bunun yerine lütfen [`Refresh`](../../pivotcache/refresh/) yöntemini kullanın ve ardından gelen [`CalculateData`](../calculatedata/) yöntemini kaldırın, çünkü bu pivot tablo [`PivotCache`](../pivotcache/) yenilenirken hesaplanacaktır. Bu yöntem Haziran 2026'dan itibaren 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRefreshDataDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);
            
            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Satır ve veri alanları ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Pivot tablo verilerini yenile ve hesapla
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableRefreshDataDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RefreshData(PivotTableRefreshOption) {#refreshdata_1}

Pivot tablonun verilerini ve ayarlarını veri kaynağından seçeneklerle yeniler.

```csharp
[Obsolete("Use PivotCache.Refresh() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotRefreshState RefreshData(PivotTableRefreshOption option)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| seçenek | PivotTableRefreshOption | Pivot tablo veri kaynağını yenileme seçenekleri. |

### Açıklamalar

Veri kaynağından pivot önbelleğine veri toplayacağız, ardından önbellekteki veriyi hücrelere hesaplayacağız. Ve dosyadaki tüm pivot tablolarını tek tek yenilemek yerine sadece [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) yöntemini çağırarak yenileyip hesaplayabilirsiniz. NOT: Bu yöntem artık kullanımdan kaldırıldı. Bunun yerine lütfen [`Refresh`](../../pivotcache/refresh/) yöntemini kullanın ve ardından gelen [`CalculateData`](../calculatedata/) yöntemini kaldırın, çünkü bu pivot tablo [`PivotCache`](../pivotcache/) yenilenirken hesaplanacaktır. Bu yöntem Haziran 2026'dan itibaren 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRefreshDataWithPivotTableRefreshOptionDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("example.xlsx");
            
            // Pivot tabloyu içeren çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets["PNL_AFS"];
            
            // Çalışma sayfasındaki ilk pivot tabloyu al
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Yenileme seçeneklerini yapılandır
            PivotTableRefreshOption refreshOptions = new PivotTableRefreshOption();
            refreshOptions.ReserveMissingPivotItemType = ReserveMissingPivotItemType.None;
            
            // Belirtilen seçeneklerle pivot tablo verilerini yenile
            pivotTable.RefreshData(refreshOptions);
            pivotTable.CalculateData();
            
            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("example_modified.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


