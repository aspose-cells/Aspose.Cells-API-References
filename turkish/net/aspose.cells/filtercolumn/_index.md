---
title: "Sınıf FilterColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FilterColumn sınıfı. Tek bir sütun veya tabloda bir sütun için filtreyi temsil eder."
type: docs
url: /tr/net/aspose.cells/filtercolumn/
---
## FilterColumn class

Tablodaki tek bir sütun veya bir sütun için bir filtreyi temsil eder.

```csharp
public class FilterColumn
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ColorFilter](../../aspose.cells/filtercolumn/colorfilter/) { get; } | Renk ile veri filtrelemek için [`ColorFilter`](../colorfilter/) alır. |
| [CustomFilters](../../aspose.cells/filtercolumn/customfilters/) { get; set; } | Özel ölçütlerle veri filtrelemek için [`CustomFilterCollection`](../customfiltercollection/) alır. |
| [DynamicFilter](../../aspose.cells/filtercolumn/dynamicfilter/) { get; } | Dinamik ölçütlerle filtrelemek için [`DynamicFilter`](./dynamicfilter/) alır. |
| [FieldIndex](../../aspose.cells/filtercolumn/fieldindex/) { get; set; } | Aralıktaki sütun kaydırmasını alır ve ayarlar. |
| [Filter](../../aspose.cells/filtercolumn/filter/) { get; set; } | (**Obsolete.**) Veri filtreleme koşulunu alır ve ayarlar. |
| [FilterType](../../aspose.cells/filtercolumn/filtertype/) { get; set; } | Veri filtreleme türünü alır ve ayarlar. |
| [FilterValues](../../aspose.cells/filtercolumn/filtervalues/) { get; } | Etiketler veya tarih saat ile veri filtrelemek için [`FilterValueCollection`](../filtervaluecollection/) alır. |
| [IconFilter](../../aspose.cells/filtercolumn/iconfilter/) { get; } | Simge ile veri filtrelemek için [`IconFilter`](./iconfilter/) alır. |
| [IsDropdownVisible](../../aspose.cells/filtercolumn/isdropdownvisible/) { get; set; } | Bu sütun için AutoFilter düğmesinin görünür olup olmadığını gösterir. |
| [MultipleFilters](../../aspose.cells/filtercolumn/multiplefilters/) { get; set; } | (**Obsolete.**) Etiketler veya tarih saat ile veri filtrelemek için [`MultipleFilterCollection`](../multiplefiltercollection/) alır. |
| [Top10Filter](../../aspose.cells/filtercolumn/top10filter/) { get; } | Veri sıralamasına göre veri filtrelemek için [`Top10Filter`](./top10filter/) alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SelectAll](../../aspose.cells/filtercolumn/selectall/)() | Tümünü seçer. |

### Örnekler

```csharp
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;

namespace AsposeCellsExamples
{
    public class FilterColumnDemo
    {
        public static void RunDemo()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Jane");
            sheet.Cells["A4"].PutValue("Doe");

            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["B3"].PutValue(25);
            sheet.Cells["B4"].PutValue(35);

            // Aralığa Otomatik Filtre Uygula
            sheet.AutoFilter.SetRange(0, 0, 3);

            // İlk sütuna (Ad) bir filtre ekle
            sheet.AutoFilter.AddFilter(0, "John");

            // İkinci sütuna (Yaş) bir filtre ekle
            sheet.AutoFilter.AddFilter(1, "30");

            // Filtreyi yenileyerek uygulayın
            sheet.AutoFilter.Refresh();

            // FilterColumnCollection'a erişin
            FilterColumnCollection filterColumns = sheet.AutoFilter.FilterColumns;

            // İlk FilterColumn'a erişin
            FilterColumn filterColumn = filterColumns[0];

            // FilterColumn'un özelliklerini göster
            Console.WriteLine($"IsDropdownVisible: {filterColumn.IsDropdownVisible}");
            Console.WriteLine($"Filter: {filterColumn.Filter}");
            Console.WriteLine($"FilterType: {filterColumn.FilterType}");
            Console.WriteLine($"FieldIndex: {filterColumn.FieldIndex}");

            // Çalışma kitabını kaydedin
            workbook.Save("FilterColumnDemo.xlsx");
            workbook.Save("FilterColumnDemo.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


