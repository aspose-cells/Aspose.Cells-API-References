---
title: "Sınıf ListObject"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Tables.ListObject sınıfı. Bir çalışma sayfasındaki tabloyu temsil eder."
type: docs
url: /tr/net/aspose.cells.tables/listobject/
---
## ListObject class

Bir çalışma sayfasındaki tabloyu temsil eder.

```csharp
public class ListObject
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AlternativeDescription](../../aspose.cells.tables/listobject/alternativedescription/) { get; set; } | Alternatif açıklamayı alır ve ayarlar. |
| [AlternativeText](../../aspose.cells.tables/listobject/alternativetext/) { get; set; } | Alternatif metni alır ve ayarlar. |
| [AutoFilter](../../aspose.cells.tables/listobject/autofilter/) { get; } | Bu tablonun otomatik filtresini alır. |
| [Comment](../../aspose.cells.tables/listobject/comment/) { get; set; } | Tablonun yorumunu alır ve ayarlar. |
| [DataRange](../../aspose.cells.tables/listobject/datarange/) { get; } | Tablonun veri aralığını alır. |
| [DataSourceType](../../aspose.cells.tables/listobject/datasourcetype/) { get; } | Tablonun veri kaynağı türünü alır. |
| [DisplayName](../../aspose.cells.tables/listobject/displayname/) { get; set; } | Tablonun görüntüleme adını alır ve ayarlar. |
| [EndColumn](../../aspose.cells.tables/listobject/endcolumn/) { get; } | Aralığın son sütununu alır. |
| [EndRow](../../aspose.cells.tables/listobject/endrow/) { get; } | Aralığın son satırını alır. |
| [HasAutoFilter](../../aspose.cells.tables/listobject/hasautofilter/) { get; set; } | Otomatik filtrenin bu tabloya uygulanıp uygulanmadığını gösterir. |
| [ListColumns](../../aspose.cells.tables/listobject/listcolumns/) { get; } | Bu tablonun [`ListColumn`](../listcolumn/) listesini alır. |
| [QueryTable](../../aspose.cells.tables/listobject/querytable/) { get; } | Bağlantılı QueryTable'ı alır. |
| [ShowHeaderRow](../../aspose.cells.tables/listobject/showheaderrow/) { get; set; } | Bu tablonun başlık satırını gösterip göstermediğini alır ve ayarlar. |
| [ShowTableStyleColumnStripes](../../aspose.cells.tables/listobject/showtablestylecolumnstripes/) { get; set; } | Sütun şerit biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [ShowTableStyleFirstColumn](../../aspose.cells.tables/listobject/showtablestylefirstcolumn/) { get; set; } | Tablodaki ilk sütunun uygulanan stil olup olmadığını gösterir. |
| [ShowTableStyleLastColumn](../../aspose.cells.tables/listobject/showtablestylelastcolumn/) { get; set; } | Tablodaki son sütunun uygulanan stil olup olmadığını gösterir. |
| [ShowTableStyleRowStripes](../../aspose.cells.tables/listobject/showtablestylerowstripes/) { get; set; } | Satır şerit biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [ShowTotals](../../aspose.cells.tables/listobject/showtotals/) { get; set; } | Bu TAble'ın toplam satırını gösterip göstermediğini alır ve ayarlar. |
| [StartColumn](../../aspose.cells.tables/listobject/startcolumn/) { get; } | Aralığın başlangıç sütununu alır. |
| [StartRow](../../aspose.cells.tables/listobject/startrow/) { get; } | Aralığın başlangıç satırını alır. |
| [TableStyleName](../../aspose.cells.tables/listobject/tablestylename/) { get; set; } | Tablo stil adını alır ve ayarlar. |
| [TableStyleType](../../aspose.cells.tables/listobject/tablestyletype/) { get; set; } | Alır ve yerleşik tablo stilini. |
| [XmlMap](../../aspose.cells.tables/listobject/xmlmap/) { get; } | Bu liste için kullanılan bir [`XmlMap`](./xmlmap/) alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [ApplyStyleToRange](../../aspose.cells.tables/listobject/applystyletorange/)() | Tablo stilini aralığa uygula. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange/#converttorange)() | Tabloyu aralığa dönüştür. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange/#converttorange_1)(TableToRangeOptions) | Tabloyu aralığa dönüştür. |
| [Filter](../../aspose.cells.tables/listobject/filter/)() | (**Obsolete.**) Tabloyu filtrele. |
| [PutCellFormula](../../aspose.cells.tables/listobject/putcellformula/#putcellformula)(int, int, string) | Formülü tablodaki hücreye koy. |
| [PutCellFormula](../../aspose.cells.tables/listobject/putcellformula/#putcellformula_1)(int, int, string, bool) | Formülü tablodaki hücreye koy. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue/#putcellvalue)(int, int, object) | Değeri hücreye koy. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue/#putcellvalue_1)(int, int, object, bool) | Değeri hücreye koy. |
| [RemoveAutoFilter](../../aspose.cells.tables/listobject/removeautofilter/)() | Bu tabloya uygulanan otomatik filtreyi kaldırır. |
| [Resize](../../aspose.cells.tables/listobject/resize/)(int, int, int, int, bool) | Liste nesnesinin aralığını yeniden boyutlandır. |
| [UpdateColumnName](../../aspose.cells.tables/listobject/updatecolumnname/)() | Tüm liste sütunlarının adını tablo içindeki hücrelere günceller. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListObjectDemo
    {
        public static void ListObjectExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Çalışma sayfasını bazı verilerle doldurun
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Çalışma sayfasına bir ListObject (tablo) ekle
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // ListObject'in bazı özelliklerini ayarla
            table.ShowTotals = true;
            table.ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;
            table.DisplayName = "SampleTable";
            table.Comment = "This is a sample table.";
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.ShowTableStyleRowStripes = true;
            table.ShowTableStyleColumnStripes = true;
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Çalışma kitabını kaydedin
            workbook.Save("ListObjectExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


