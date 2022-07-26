---
title: ListObject
second_title: Aspose.Cells for .NET API Referansı
description: Çalışma sayfasındaki bir liste nesnesini temsil eder. ListObject nesnesi ListObjects koleksiyonunun bir üyesidir. ListObjects koleksiyonu bir çalışma sayfasındaki tüm liste nesnelerini içerir.
type: docs
weight: 5820
url: /tr/net/aspose.cells.tables/listobject/
---
## ListObject class

Çalışma sayfasındaki bir liste nesnesini temsil eder. ListObject nesnesi, ListObjects koleksiyonunun bir üyesidir. ListObjects koleksiyonu, bir çalışma sayfasındaki tüm liste nesnelerini içerir.

```csharp
public class ListObject
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AlternativeDescription](../../aspose.cells.tables/listobject/alternativedescription) { get; set; } | Alternatif açıklamayı alır ve ayarlar. |
| [AlternativeText](../../aspose.cells.tables/listobject/alternativetext) { get; set; } | Alternatif metni alır ve ayarlar. |
| [AutoFilter](../../aspose.cells.tables/listobject/autofilter) { get; } | Otomatik filtre alır. |
| [Comment](../../aspose.cells.tables/listobject/comment) { get; set; } | Tablonun yorumunu alır ve ayarlar. |
| [DataRange](../../aspose.cells.tables/listobject/datarange) { get; } | ListObject. veri aralığını alır |
| [DataSourceType](../../aspose.cells.tables/listobject/datasourcetype) { get; } | Tablonun veri kaynağı türünü alır. |
| [DisplayName](../../aspose.cells.tables/listobject/displayname) { get; set; } | Görünen adı alır ve ayarlar. |
| [EndColumn](../../aspose.cells.tables/listobject/endcolumn) { get; } | Aralığın bitiş sütununu alır. |
| [EndRow](../../aspose.cells.tables/listobject/endrow) { get; } | Aralığın son satırını alır. |
| [ListColumns](../../aspose.cells.tables/listobject/listcolumns) { get; } | ListObject'in ListColumns'unu alır. |
| [QueryTable](../../aspose.cells.tables/listobject/querytable) { get; } | Bağlantılı QueryTable'ı alır. |
| [ShowHeaderRow](../../aspose.cells.tables/listobject/showheaderrow) { get; set; } | Bu ListObject'in başlık satırını gösterip göstermediğini alır ve ayarlar. |
| [ShowTableStyleColumnStripes](../../aspose.cells.tables/listobject/showtablestylecolumnstripes) { get; set; } | Sütun şerit biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [ShowTableStyleFirstColumn](../../aspose.cells.tables/listobject/showtablestylefirstcolumn) { get; set; } | Tablodaki ilk sütuna stilin uygulanıp uygulanmayacağını belirtir. |
| [ShowTableStyleLastColumn](../../aspose.cells.tables/listobject/showtablestylelastcolumn) { get; set; } | Tablodaki son sütuna stilin uygulanıp uygulanmayacağını belirtir. |
| [ShowTableStyleRowStripes](../../aspose.cells.tables/listobject/showtablestylerowstripes) { get; set; } | Satır şerit biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [ShowTotals](../../aspose.cells.tables/listobject/showtotals) { get; set; } | Bu ListObject'in toplam satırı gösterip göstermediğini alır ve ayarlar. |
| [StartColumn](../../aspose.cells.tables/listobject/startcolumn) { get; } | Aralığın başlangıç sütununu alır. |
| [StartRow](../../aspose.cells.tables/listobject/startrow) { get; } | Aralığın başlangıç satırını alır. |
| [TableStyleName](../../aspose.cells.tables/listobject/tablestylename) { get; set; } | Tablo stili adını alır ve ayarlar. |
| [TableStyleType](../../aspose.cells.tables/listobject/tablestyletype) { get; set; } | Gets ve yerleşik tablo stili. |
| [XmlMap](../../aspose.cells.tables/listobject/xmlmap) { get; } | Bir[`XmlMap`](./xmlmap)bu liste için kullanılır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [ApplyStyleToRange](../../aspose.cells.tables/listobject/applystyletorange)() | Tablo stilini aralığa uygulayın. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange#converttorange)() | Tabloyu aralığa dönüştürün. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange#converttorange_1)(TableToRangeOptions) | Tabloyu aralığa dönüştürün. |
| [Filter](../../aspose.cells.tables/listobject/filter)() | Tabloyu filtreleyin. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue)(int, int, object) | Değeri hücreye koyun. |
| [Resize](../../aspose.cells.tables/listobject/resize)(int, int, int, int, bool) | Liste nesnesinin aralığını yeniden boyutlandırın. |
| [UpdateColumnName](../../aspose.cells.tables/listobject/updatecolumnname)() | Çalışma sayfasından tüm liste sütunlarının adını günceller. |

### Örnekler

```csharp

[C#]


Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
for (int i = 0; i  <5; i++)
{
cells[0,i].PutValue(CellsHelper.ColumnIndexToName(i));
 }
for (int row = 1; row  <10; row++)
{
 for (int column = 0; column  <5; column++)
{
cells[row, column].PutValue(row * column);
 }
 }
ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
int index = tables.Add(0, 0, 9, 4, true);
ListObject table = tables[0];
table.ShowTotals = true;
table.ListColumns[4].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
workbook.Save(@"Book1.xlsx");


[Visual Basic]

Dim workbook As Workbook = New Workbook()
Dim cells As Cells = workbook.Worksheets(0).Cells
For i As Int32 = 0 To 4
 cells(0, i).PutValue(CellsHelper.ColumnIndexToName(i))
Next
For row As Int32 = 1 To 9
 For column As Int32 = 0 To 4
  cells(row, column).PutValue(row * column)
Next
Next
Dim tables As ListObjectCollection = workbook.Worksheets(0).ListObjects
Dim index As Int32 = tables.Add(0, 0, 9, 4, True)
Dim table As ListObject = tables(0)
table.ShowTotals = True
table.ListColumns(4).TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum
workbook.Save("Book1.xlsx")
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells.Tables](../../aspose.cells.tables)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
