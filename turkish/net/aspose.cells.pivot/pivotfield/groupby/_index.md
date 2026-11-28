---
title: "PivotField.GroupBy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField yöntemi. Alanı aralıkla otomatik olarak grupla"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/groupby/
---
## GroupBy(double, bool) {#groupby_7}

Alanı aralıkla otomatik olarak grupla

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GroupBy(double interval, bool newField)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aralık | Double | Grubun iç değeri. Sıfır ise otomatik değer atanır, |
| newField | Boolean | Pivot tabloya yeni bir alan eklenip eklenmediğini gösterir. Yalnızca DateTime gruplaması için. |

### Açıklamalar

NOTE: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotField.Group(PivotFieldGroupOptions) yöntemini kullanın. Bu yöntem, Eylül 2026'dan itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGroupByWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("example.xlsx");
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İlk pivot tabloya eriş
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Alanı sütun alanına ekle
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, 2);
            
            // Alanı 1 (aralık) ile otomatik aralıkta grupla
            pivotTable.BaseFields[2].GroupBy(1.0, true);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(PivotGroupByType[], double, bool) {#groupby_6}

Alanı internal ile otomatik olarak grupla

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GroupBy(PivotGroupByType[] groups, double interval, bool newField)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| gruplar | PivotGroupByType[] | Grup türleri |
| aralık | Double | Grubun iç değeri. Sıfır ise otomatik değer atanır, yalnızca Sayılar veya Günler ile gruplama için çalışır. |
| newField | Boolean | Pivot tabloya yeni bir alan eklenip eklenmediğini gösterir. |

### Açıklamalar

NOTE: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotField.Group(PivotFieldGroupOptions) yöntemini kullanın. Bu yöntem, Eylül 2026'dan itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Ayrıca Bakınız

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(DateTime, DateTime, PivotGroupByType[], double, bool) {#groupby_5}

Dosyayı tarih grup türlerine göre gruplayın.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(DateTime start, DateTime end, PivotGroupByType[] groups, double interval, 
    bool firstAsNewField)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlangıç | DateTime | Başlangıç tarih ve saati |
| bitiş | DateTime | Tarih ve saat sonu |
| gruplar | PivotGroupByType[] | Grup türleri |
| aralık | Double | Aralık |
| firstAsNewField | Boolean | Pivot tabloya yeni bir alan eklenip eklenmeyeceğini gösterir. Yalnızca ilk grup öğesi için. |

### Dönüş Değeri

False, bu alanın tarih ve saate göre gruplanamayacağını gösterir.

### Açıklamalar

NOTE: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotField.Group(PivotFieldGroupOptions) yöntemini kullanın. Bu yöntem, Eylül 2026'dan itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGroupByWithDateTimeDateTimePivotGroupByTyDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pivot tablo için tarih içeren örnek veri ekleyin
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 15);
            worksheet.Cells["A3"].Value = new DateTime(2023, 2, 20);
            worksheet.Cells["A4"].Value = new DateTime(2023, 3, 10);
            worksheet.Cells["A5"].Value = new DateTime(2023, 4, 5);
            worksheet.Cells["A6"].Value = new DateTime(2023, 5, 25);
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1500;
            worksheet.Cells["B3"].Value = 2300;
            worksheet.Cells["B4"].Value = 3200;
            worksheet.Cells["B5"].Value = 4100;
            worksheet.Cells["B6"].Value = 5000;

            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            
            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Pivot alanını al
            PivotField pivotField = pivotTable.RowFields[0];

            // GroupBy yöntemi için parametreleri hazırlayın
            DateTime startDate = new DateTime(2023, 1, 1);
            DateTime endDate = new DateTime(2023, 6, 30);
            PivotGroupByType[] groupTypes = new PivotGroupByType[] { PivotGroupByType.Months };
            double interval = 1;
            bool firstAsNewField = false;

            try
            {
                // GroupBy yöntemini tarih parametreleriyle çağırın
                bool result = pivotField.GroupBy(startDate, endDate, groupTypes, interval, firstAsNewField);
                
                Console.WriteLine("GroupBy method executed successfully. Result: " + result);
                
                // Pivot tabloyu yenile
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GroupBy method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotFieldGroupByDateTimeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(bool, DateTime, bool, DateTime, PivotGroupByType[], double, bool) {#groupby_3}

Dosyayı tarih grup türlerine göre gruplayın.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(bool isAutoStart, DateTime start, bool isAutoEnd, DateTime end, 
    PivotGroupByType[] groups, double interval, bool firstAsNewField)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isAutoStart | Boolean | Başlangıç tarih ve saat değerinin otomatik algılanıp algılanmayacağını gösterir. |
| başlangıç | DateTime | Başlangıç tarih ve saati |
| isAutoEnd | Boolean | Bitiş tarih ve saat değerinin otomatik algılanıp algılanmayacağını gösterir. |
| bitiş | DateTime | Tarih ve saat sonu |
| gruplar | PivotGroupByType[] | Grup türleri |
| aralık | Double | Aralık |
| firstAsNewField | Boolean | Pivot tabloya yeni bir alan eklenip eklenmeyeceğini gösterir. Yalnızca ilk grup öğesi için. |

### Dönüş Değeri

False, bu alanın tarih ve saate göre gruplanamayacağını gösterir.

### Açıklamalar

NOTE: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotField.Group(PivotFieldGroupOptions) yöntemini kullanın. Bu yöntem, Eylül 2026'dan itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Ayrıca Bakınız

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(double, double, double, bool) {#groupby_4}

Dosyayı sayıya göre gruplayın.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(double start, double end, double interval, bool newField)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlangıç | Double | Başlangıç değeri |
| bitiş | Double | Değerin sonu |
| aralık | Double | Aralık |
| newField | Boolean | Pivot tabloya yeni bir alan eklenip eklenmeyeceğini gösterir |

### Dönüş Değeri

False, bu alanın tarih ve saate göre gruplanamayacağını gösterir.

### Açıklamalar

NOTE: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotField.Group(PivotFieldGroupOptions) yöntemini kullanın. Bu yöntem, Eylül 2026'dan itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGroupByWithDoubleDoubleDoubleBooleanDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Value";
            worksheet.Cells["A2"].Value = 1;
            worksheet.Cells["A3"].Value = 2;
            worksheet.Cells["A4"].Value = 3;
            worksheet.Cells["A5"].Value = 4;
            worksheet.Cells["A6"].Value = 5;
            worksheet.Cells["A7"].Value = 6;

            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:A7", "D1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Satır alanı ekleyin ve gruplayın
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField rowField = pivotTable.RowFields[fieldIndex];
            rowField.GroupBy(1, 6, 2, false); // Group values from 1 to 6 with interval 2, auto range false
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotGroupByExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(bool, double, bool, double, double, bool) {#groupby_2}

Dosyayı sayıya göre gruplayın.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(bool isAutoStart, double start, bool isAutoEnd, double end, double interval, 
    bool newField)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isAutoStart | Boolean | Başlangıç değerinin otomatik algılanıp algılanmayacağını gösterir. |
| başlangıç | Double | Başlangıç değeri |
| isAutoEnd | Boolean | Bitiş değerinin otomatik algılanıp algılanmayacağını gösterir. |
| bitiş | Double | Değerin sonu |
| aralık | Double | Aralık |
| newField | Boolean | Pivot tabloya yeni bir alan eklenip eklenmeyeceğini gösterir |

### Dönüş Değeri

False, bu alanın tarih ve saate göre gruplanamayacağını gösterir.

### Açıklamalar

NOTE: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotField.Group(PivotFieldGroupOptions) yöntemini kullanın. Bu yöntem, Eylül 2026'dan itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(CustomPiovtFieldGroupItem[], bool) {#groupby}

Alanı özel olarak gruplayın.

```csharp
[Obsolete("Use PivotField.Group(PivotFieldGroupOptions options) method with PivotFieldGroupOptions.DiscreteGroupItems property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(CustomPiovtFieldGroupItem[] customGroupItems, bool newField)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| customGroupItems | CustomPiovtFieldGroupItem[] | Özel grup öğeleri. |
| newField | Boolean | Pivot tabloya yeni bir alan eklenip eklenmeyeceğini gösterir |

### Dönüş Değeri

False, bu alanın tarih ve saate göre gruplanamayacağını gösterir.

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.Group(PivotFieldGroupOptions options) yöntemini PivotFieldGroupOptions.DiscreteGroupItems özelliği ile kullanın. Bu yöntem Temmuz 2026'dan itibaren 6 ay içinde kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGroupByWithCustomPiovtFieldGroupItemBooDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["A5"].Value = "Grapes";
            worksheet.Cells["A6"].Value = "Mango";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;
            worksheet.Cells["B5"].Value = 4000;
            worksheet.Cells["B6"].Value = 5000;

            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Pivot alanını al
            PivotField pivotField = pivotTable.RowFields[0];

            // Özel grup öğeleri oluştur
            CustomPiovtFieldGroupItem[] customGroupItems = new CustomPiovtFieldGroupItem[2];
            customGroupItems[0] = new CustomPiovtFieldGroupItem("Group1", new int[] { 0, 1 }); // Apple (index 0), Banana (index 1)
            customGroupItems[1] = new CustomPiovtFieldGroupItem("Group2", new int[] { 2, 3, 4 }); // Orange (2), Grapes (3), Mango (4)

            try
            {
                // Özel grup öğeleriyle GroupBy yöntemini çağırın
                bool result = pivotField.GroupBy(customGroupItems, false);
                
                Console.WriteLine("GroupBy method executed successfully. Result: " + result);
                
                // Pivot tabloyu yenile
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GroupBy method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotFieldGroupByCustomDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomPiovtFieldGroupItem](../../custompiovtfieldgroupitem/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(DiscreteGroupItem[], bool) {#groupby_1}

Alanı özel olarak gruplayın.

```csharp
[Obsolete("Use PivotField.Group(PivotFieldGroupOptions options) method with PivotFieldGroupOptions.DiscreteGroupItems property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(DiscreteGroupItem[] customGroupItems, bool newField)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| customGroupItems | DiscreteGroupItem[] | Özel grup öğeleri. |
| newField | Boolean | Pivot tabloya yeni bir alan eklenip eklenmeyeceğini gösterir |

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.Group(PivotFieldGroupOptions options) yöntemini PivotFieldGroupOptions.DiscreteGroupItems özelliği ile kullanın. Bu yöntem Temmuz 2026'dan itibaren 6 ay içinde kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Ayrıca Bakınız

* class [DiscreteGroupItem](../../discretegroupitem/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


