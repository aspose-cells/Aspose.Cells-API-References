---
title: "Sınıf PivotFieldGroupOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.PivotFieldGroupOptions sınıfı. Özet alanı gruplama ayarları için seçenekler"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfieldgroupoptions/
---
## PivotFieldGroupOptions class

Pivot alanı gruplama ayarları için seçenekler.

```csharp
public class PivotFieldGroupOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PivotFieldGroupOptions](pivotfieldgroupoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [DiscreteGroupItems](../../aspose.cells.pivot/pivotfieldgroupoptions/discretegroupitems/) { get; set; } | Ayrık grup öğelerini alır ve ayarlar. |
| [EndDate](../../aspose.cells.pivot/pivotfieldgroupoptions/enddate/) { get; set; } | Gruplama aralığının bitiş değerini alır veya ayarlar. |
| [EndNumber](../../aspose.cells.pivot/pivotfieldgroupoptions/endnumber/) { get; set; } | Gruplama aralığının bitiş değerini alır veya ayarlar. |
| [GroupType](../../aspose.cells.pivot/pivotfieldgroupoptions/grouptype/) { get; set; } | Özet alanı için gruplama türünü alır veya ayarlar. Yalnızca tarih saat özet alanı gruplaması için. |
| [GroupTypes](../../aspose.cells.pivot/pivotfieldgroupoptions/grouptypes/) { get; set; } | Özet alanı için gruplama türünü alır veya ayarlar. |
| [Interval](../../aspose.cells.pivot/pivotfieldgroupoptions/interval/) { get; set; } | Her grup için aralık boyutunu alır veya ayarlar. |
| [IsAutoEnd](../../aspose.cells.pivot/pivotfieldgroupoptions/isautoend/) { get; set; } | Bitiş değerinin otomatik olarak belirlenip belirlenmediğini gösteren bir değeri alır veya ayarlar. |
| [IsAutoStart](../../aspose.cells.pivot/pivotfieldgroupoptions/isautostart/) { get; set; } | Başlangıç değerinin otomatik olarak belirlenip belirlenmediğini gösteren bir değeri alır veya ayarlar. |
| [NewPivotField](../../aspose.cells.pivot/pivotfieldgroupoptions/newpivotfield/) { get; set; } | Gruplamadan sonra yeni özet alanlarının oluşturulup oluşturulmayacağını gösteren bir değeri alır veya ayarlar. |
| [StartDate](../../aspose.cells.pivot/pivotfieldgroupoptions/startdate/) { get; set; } | Gruplama aralığının başlangıç değerini alır veya ayarlar. |
| [StartNumber](../../aspose.cells.pivot/pivotfieldgroupoptions/startnumber/) { get; set; } | Gruplama aralığının başlangıç değerini alır veya ayarlar. |

### Örnekler

```csharp

[C#]

// Örnek çalışma kitabını yükle
Workbook wb = new Workbook("sampleGroupPivotFieldsInPivotTable.xlsx");
// İkinci çalışma sayfasına ve onun özet tablosuna eriş
PivotTable pt = wb.Worksheets[1].PivotTables[0];
// İlk satır alanını (bir tarih alanı) aylar ve çeyrekler bazında grupla
PivotFieldGroupOptions options = new PivotFieldGroupOptions();
options.StartDate = new DateTime(2008, 1, 1);
options.EndDate = new DateTime(2008, 9, 5);
options.GroupTypes = new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Quarters };
pt.RowFields[0].Group(options);
// Pivot tablo verilerini hesaplayın ve çıktı dosyasını kaydedin
pt.CalculateData();
wb.Save("outputGroupPivotFieldsInPivotTable.xlsx");

[Visual Basic]

'Load the sample workbook
Dim wb As New Workbook("sampleGroupPivotFieldsInPivotTable.xlsx")
'Access the second worksheet and its pivot table
Dim pt As PivotTable = wb.Worksheets(1).PivotTables(0)
'Group the first row field (a date field) by months and quarters
Dim options As New PivotFieldGroupOptions()
options.StartDate = New DateTime(2008, 1, 1)
options.EndDate = New DateTime(2008, 9, 5)
options.GroupTypes = New PivotGroupByType() {PivotGroupByType.Months, PivotGroupByType.Quarters}
pt.RowFields(0).Group(options)
'Calculate the pivot table data and save the output file
pt.CalculateData()
wb.Save("outputGroupPivotFieldsInPivotTable.xlsx")
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


