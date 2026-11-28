---
title: "PivotField.SortBy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField yöntemi. Bu pivot alanını sıralar"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/sortby/
---
## SortBy(SortOrder) {#sortby}

Bu pivot alanını sıralar.

```csharp
public void SortBy(SortOrder sortType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sortType | SortOrder | Bu alanın sıralama türü. |

### Ayrıca Bakınız

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int) {#sortby_1}

Bu pivot alanını sıralar.

```csharp
[Obsolete("Use PivotField.SortBy(SortOrder, int,string) method or PivotField.IsAutoSort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SortBy(SortOrder sortType, int fieldSortedBy)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sortType | SortOrder | Bu alanın sıralama türü. |
| fieldSortedBy | Int32 | Sıralama yapılan pivot alanının indeksi. -1, bu alanın veri etiketlerine göre sıralama anlamına gelir, diğer değerler sıralama yapılan veri alanının indeksini gösterir. |

### Açıklamalar

NOT: Bu özellik artık eski. Bunun yerine, lütfen PivotField.SortBy(SortOrder, int,string) yöntemini veya PivotField.IsAutoSort özelliğini kullanın. Bu yöntem, Eylül 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSortByWithSortOrderInt32Demo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("UK");
            worksheet.Cells["A4"].PutValue("Germany");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(1500);

            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Satır alanı ekle
            int rowIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            PivotField rowField = pivotTable.RowFields[rowIndex];
            
            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Satır alanını -1 indeksle azalan sırada sıralayın
            rowField.SortBy(SortOrder.Descending, -1);
            
            // Özet tabloyu yenile ve hesapla
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotFieldSortByDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int, PivotLineType, string) {#sortby_2}

Bu pivot alanını sıralar.

```csharp
[Obsolete("Use PivotField.SortBy(SortOrder, int,string) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SortBy(SortOrder sortType, int fieldSortedBy, PivotLineType dataType, string cellName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sortType | SortOrder | Bu alanın sıralama türü. |
| fieldSortedBy | Int32 | Sıralama yapılan pivot alanının indeksi. -1, bu alanın veri etiketlerine göre sıralama anlamına gelir, diğer değerler sıralama yapılan veri alanının indeksini gösterir. |
| dataType | PivotLineType | Sıralanan veri türü. |
| cellName | String | Satır veya sütundaki değerlere göre sırala |

### Açıklamalar

NOT: Bu özellik artık eski. Bunun yerine, lütfen PivotField.SortBy(SortOrder, int,string) yöntemini kullanın. Bu yöntem, Eylül 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSortByWithSortOrderInt32PivotLineTypeStrDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("B");
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["B3"].PutValue(300);
            worksheet.Cells["B4"].PutValue(100);

            // Özet tablo oluştur
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Satır alanını sırala
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "E4");
            
            // Verileri hesapla
            pivotTable.CalculateData();
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotFieldSortByDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [SortOrder](../../../aspose.cells/sortorder/)
* enum [PivotLineType](../../pivotlinetype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int, string) {#sortby_3}

Bu pivot alanını sıralar.

```csharp
public void SortBy(SortOrder sortType, int fieldSortedBy, string cellName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sortType | SortOrder | Bu alanın sıralama türü. |
| fieldSortedBy | Int32 | Sıralama yapılan pivot alanının indeksi. -1, bu alanın veri etiketlerine göre sıralama anlamına gelir, diğer değerler sıralama yapılan veri alanının indeksini gösterir. |
| cellName | String | Satır veya sütundaki değerlere göre sırala. Null ise, alanın toplamına göre grupla; aksi takdirde seçilen sütun veya satırdaki değerlere göre grupla. |

### Ayrıca Bakınız

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


