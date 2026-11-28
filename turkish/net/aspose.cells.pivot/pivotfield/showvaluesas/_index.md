---
title: "PivotField.ShowValuesAs"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField yöntemi. ShowDataAs hesabı kullanıldığında veri alanının değerlerini farklı bir görüntüleme biçimi olarak gösterir"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/showvaluesas/
---
## ShowValuesAs(PivotFieldDataDisplayFormat, int, PivotItemPositionType, int) {#showvaluesas}

ShowDataAs hesabı kullanıldığında veri alanının değerlerini farklı bir görüntüleme biçimi olarak gösterir.

```csharp
[Obsolete("Use PivotField.ShowValuesAs(PivotShowValuesAsType,int int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ShowValuesAs(PivotFieldDataDisplayFormat displayFormat, int baseField, 
    PivotItemPositionType baseItemPositionType, int baseItem)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| displayFormat | PivotFieldDataDisplayFormat | Veri görüntüleme biçimi türü. |
| baseField | Int32 | ShowDataAs hesaplamasının dayandığı alanın indeksi. |
| baseItemPositionType | PivotItemPositionType | Temel öğenin konum türü. |
| baseItem | Int32 | ShowDataAs hesaplamasının dayandığı temel öğenin indeksi. Yalnızca baseItemPositionType özelleştirilmiş olduğunda çalışır. |

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotField.ShowValuesAs(PivotShowValuesAsType,int,int) yöntemini kullanın. Bu yöntem, Kasım 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodShowValuesAsWithPivotFieldDataDisplayFormatIntDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[workbook.Worksheets.Add()];
            worksheet.Name = "PivotData";

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Quarter");
            worksheet.Cells["C1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["B2"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue(1000);
            
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue(1500);
            
            worksheet.Cells["A4"].PutValue("Furniture");
            worksheet.Cells["B4"].PutValue("Q1");
            worksheet.Cells["C4"].PutValue(800);
            
            worksheet.Cells["A5"].PutValue("Furniture");
            worksheet.Cells["B5"].PutValue("Q2");
            worksheet.Cells["C5"].PutValue(1200);

            // Özet tablo oluştur
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=PivotData!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Satır alanı ekle
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields[rowFieldIndex];

            // Sütun alanı ekle
            int columnFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, "Quarter");
            PivotField columnField = pivotTable.ColumnFields[columnFieldIndex];

            // Veri alanı ekle ve ShowValuesAs'i yapılandır
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[dataFieldIndex];
            dataField.DisplayName = "Sales Diff";
            dataField.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, columnField.BaseIndex, PivotItemPositionType.Next, 0);

            // Verileri hesaplayın ve kaydedin
            pivotTable.CalculateData();
            workbook.Save("PivotTableShowValuesAsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* enum [PivotItemPositionType](../../pivotitempositiontype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## ShowValuesAs(PivotShowValuesAsType, int, int) {#showvaluesas_1}

Bu pivot alanı için \"Show Values As\" hesaplamasını ayarlar.

```csharp
public void ShowValuesAs(PivotShowValuesAsType showValuesAsType, int baseField, int baseItem)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | "Show Values As" hesaplamasının türü. |
| baseField | Int32 | Hesaplama için kullanılan temel alanın indeksi. |
| baseItem | Int32 | Hesaplama için temel öğenin indeksi. Önceki öğe için [`PreviousPivotItem`](../../pivotshowvaluessetting/previouspivotitem/) (-1), sonraki öğe için [`NextPivotItem`](../../pivotshowvaluessetting/nextpivotitem/) (-2) kullanın; negatif olmayan değerler belirli bir pivot öğesinin sıralı indeksini gösterir. |

### Açıklamalar

Yalnızca veri alanı için.

### Ayrıca Bakınız

* enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## ShowValuesAs(PivotShowValuesAsType, string, string) {#showvaluesas_2}

Bu veri alanı için \"Show Values As\" hesaplamasını yapılandırır.

```csharp
public void ShowValuesAs(PivotShowValuesAsType showValuesAsType, string baseField, string baseItem)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | "Show Values As" için hesaplama türü. |
| baseField | String | Hesaplamada kullanılan temel alanın adı. |
| baseItem | String | Normal bir pivot öğesinin başlığı. Ayrıca ayrılmış kelime anahtarlarını kabul eder: önceki öğe için `(previous)`, sonraki öğe için `(next)`. Seçilen hesaplama türü bir temel öğe gerektirmiyorsa `null` geçirin. |

### Ayrıca Bakınız

* enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


