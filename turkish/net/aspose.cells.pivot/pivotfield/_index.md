---
title: PivotField
second_title: Aspose.Cells for .NET API Referansı
description: PivotTable raporundaki bir alanı temsil eder.
type: docs
weight: 4530
url: /tr/net/aspose.cells.pivot/pivotfield/
---
## PivotField class

PivotTable raporundaki bir alanı temsil eder.

```csharp
public class PivotField
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AutoShowCount](../../aspose.cells.pivot/pivotfield/autoshowcount) { get; set; } | Belirtilen PivotTable alanında otomatik olarak gösterilen üst veya alt öğelerin sayısını temsil eder. |
| [AutoShowField](../../aspose.cells.pivot/pivotfield/autoshowfield) { get; set; } | Otomatik gösteri alanı dizinini temsil eder. -1, PivotField'in kendisi anlamına gelir. Veri alanlarının dizini olmalıdır. |
| [AutoSortField](../../aspose.cells.pivot/pivotfield/autosortfield) { get; set; } | Otomatik sıralama alanı dizinini temsil eder. -1, PivotField'in kendisi anlamına gelir, diğerleri ise veri alanlarının konumu anlamına gelir. |
| [BaseFieldIndex](../../aspose.cells.pivot/pivotfield/basefieldindex) { get; set; } | Özel bir hesaplama için temel alanı temsil eder. |
| [BaseIndex](../../aspose.cells.pivot/pivotfield/baseindex) { get; set; } | Temel PivotFields. içindeki PivotField dizinini temsil eder |
| [BaseItemIndex](../../aspose.cells.pivot/pivotfield/baseitemindex) { get; set; } | Özel bir hesaplama için temel alandaki öğeyi temsil eder. Yalnızca veri alanları için geçerlidir. |
| [BaseItemPosition](../../aspose.cells.pivot/pivotfield/baseitemposition) { get; set; } | Özel bir hesaplama için temel alandaki öğeyi temsil eder. Yalnızca veri alanları için geçerlidir. PivotItemPosition.Custom yalnızca okuma için olduğundan, PivotItemPosition.Custom, ayarlamanız gerekiyorsa lütfen PivotField.BaseItemIndex özniteliğini ayarlayın. |
| [CurrentPageItem](../../aspose.cells.pivot/pivotfield/currentpageitem) { get; set; } | Sayfa alanı için gösterilen geçerli sayfa öğesini temsil eder (yalnızca sayfa alanları için geçerlidir). |
| [DataDisplayFormat](../../aspose.cells.pivot/pivotfield/datadisplayformat) { get; set; } | Bir veri alanında bulunan değerlerin nasıl görüntüleneceğini temsil eder. |
| [DisplayName](../../aspose.cells.pivot/pivotfield/displayname) { get; set; } | PivotField görünen adını temsil eder. |
| [DragToColumn](../../aspose.cells.pivot/pivotfield/dragtocolumn) { get; set; } | Belirtilen alanın sütun konumuna sürüklenip sürüklenmeyeceğini gösterir. Varsayılan değer true'dur. |
| [DragToData](../../aspose.cells.pivot/pivotfield/dragtodata) { get; set; } | Belirtilen alanın veri konumuna sürüklenip sürüklenmeyeceğini gösterir. Varsayılan değer doğrudur. |
| [DragToHide](../../aspose.cells.pivot/pivotfield/dragtohide) { get; set; } | Belirtilen alanın gizleme konumuna sürüklenip sürüklenmeyeceğini gösterir. Varsayılan değer true'dur. |
| [DragToPage](../../aspose.cells.pivot/pivotfield/dragtopage) { get; set; } | Belirtilen alanın sayfa konumuna sürüklenip sürüklenmeyeceğini gösterir. Varsayılan değer doğrudur. |
| [DragToRow](../../aspose.cells.pivot/pivotfield/dragtorow) { get; set; } | Belirtilen alanın satır konumuna sürüklenip sürüklenmeyeceğini gösterir. Varsayılan değer doğrudur. |
| [Function](../../aspose.cells.pivot/pivotfield/function) { get; set; } | PivotTable veri alanını özetlemek için kullanılan işlevi temsil eder. |
| [InsertBlankRow](../../aspose.cells.pivot/pivotfield/insertblankrow) { get; set; } | Her öğeden sonra boş satır eklenip eklenmeyeceğini belirtir. |
| [IsAscendShow](../../aspose.cells.pivot/pivotfield/isascendshow) { get; set; } | Belirtilen PivotTable alanının artan şekilde otomatik gösterilip gösterilmediğini gösterir. |
| [IsAscendSort](../../aspose.cells.pivot/pivotfield/isascendsort) { get; set; } | Belirtilen PivotTable alanının artan şekilde otomatik olarak sıralanıp sıralanmadığını gösterir. |
| [IsAutoShow](../../aspose.cells.pivot/pivotfield/isautoshow) { get; set; } | Belirtilen PivotTable alanının otomatik olarak gösterilip gösterilmediğini belirtir, yalnızca excel 2003 için geçerlidir. |
| [IsAutoSort](../../aspose.cells.pivot/pivotfield/isautosort) { get; set; } | Belirtilen PivotTable alanının otomatik olarak sıralanıp sıralanmadığını gösterir. |
| [IsAutoSubtotals](../../aspose.cells.pivot/pivotfield/isautosubtotals) { get; set; } | Belirtilen alanın otomatik alt toplamları gösterip göstermediğini gösterir. Varsayılan true. |
| [IsCalculatedField](../../aspose.cells.pivot/pivotfield/iscalculatedfield) { get; } | Belirtilen PivotTable alanının hesaplanmış alan olup olmadığını gösterir. |
| [IsIncludeNewItemsInFilter](../../aspose.cells.pivot/pivotfield/isincludenewitemsinfilter) { get; set; } | , alanın manuel filtreye yeni öğeler dahil edip edemeyeceğini gösterir Varsayılan değer yanlıştır. |
| [IsInsertPageBreaksBetweenItems](../../aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems) { get; set; } | , alanın öğeler arasına sayfa sonları ekleyip ekleyemeyeceğini belirtir her öğeden sonra sayfa sonu ekle Varsayılan değer yanlıştır. |
| [IsMultipleItemSelectionAllowed](../../aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed) { get; set; } | , alanın field sayfasında seçilen birden çok öğeye sahip olup olamayacağını belirtir Varsayılan değer false'tur. |
| [IsRepeatItemLabels](../../aspose.cells.pivot/pivotfield/isrepeatitemlabels) { get; set; } | alanın öğeleri tekrar edip edemeyeceğini belirtir labels Varsayılan değer false'tur. |
| [ItemCount](../../aspose.cells.pivot/pivotfield/itemcount) { get; } | Bu pivot alanın temel öğe sayısını alır. |
| [Items](../../aspose.cells.pivot/pivotfield/items) { get; } | Tüm temel öğeleri alın; |
| [Name](../../aspose.cells.pivot/pivotfield/name) { get; } | PivotField adını temsil eder. |
| [Number](../../aspose.cells.pivot/pivotfield/number) { get; set; } | Sayıların ve tarihlerin yerleşik görüntüleme biçimini temsil eder. |
| [NumberFormat](../../aspose.cells.pivot/pivotfield/numberformat) { get; set; } | Sayıların ve tarihlerin özel görüntüleme biçimini temsil eder. |
| [OriginalItems](../../aspose.cells.pivot/pivotfield/originalitems) { get; } | Orijinal temel öğeleri alın; |
| [PivotItems](../../aspose.cells.pivot/pivotfield/pivotitems) { get; } | Özet alanının özet öğelerini alır |
| [Position](../../aspose.cells.pivot/pivotfield/position) { get; } | PivotFields. içindeki PivotField dizinini temsil eder |
| [Range](../../aspose.cells.pivot/pivotfield/range) { get; } | Pivot alanının grup aralığını alır |
| [ShowAllItems](../../aspose.cells.pivot/pivotfield/showallitems) { get; set; } | Özet veri içermeseler bile PivotTable raporundaki tüm öğelerin görüntülenip görüntülenmeyeceğini belirtir. veri içermeyen öğeleri göster Varsayılan değer yanlıştır. |
| [ShowCompact](../../aspose.cells.pivot/pivotfield/showcompact) { get; set; } | Özet Tablo görünümünde aynı sütunda bir sonraki alandan etiketlerin görüntülenip görüntülenmeyeceğini belirtir |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivotfield/showinoutlineform) { get; set; } | Bu alanın Özet Tablo görünümünde anahat biçiminde düzenlenip düzenlenmediğini gösterir |
| [ShowSubtotalAtTop](../../aspose.cells.pivot/pivotfield/showsubtotalattop) { get; set; } | ShowInOutlineForm doğru olduğunda, alt toplamları öğe listesinin alt kısmı yerine en üstünde görüntüleyin |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [AddCalculatedItem](../../aspose.cells.pivot/pivotfield/addcalculateditem)(string, string) | Özet alanına hesaplanmış bir öğe ekleyin. |
| [GetCalculatedFieldFormula](../../aspose.cells.pivot/pivotfield/getcalculatedfieldformula)() | Belirtilen hesaplanan alanın formül dizesini alın . |
| [GetPivotFilterByType](../../aspose.cells.pivot/pivotfield/getpivotfilterbytype)(PivotFilterType) | type ile özet alanının özet filtresini alır |
| [GetPivotFilters](../../aspose.cells.pivot/pivotfield/getpivotfilters)() | özet alanının özet filtrelerini alır |
| [GetSubtotals](../../aspose.cells.pivot/pivotfield/getsubtotals)(PivotFieldSubtotalType) | Belirtilen alanın bu alt toplamları gösterip göstermediğini alır. |
| [HideDetail](../../aspose.cells.pivot/pivotfield/hidedetail)(bool) | Bir pivot alanındaki PivotItems'in gizli ayrıntı olup olmadığını ayarlar. Bu, bu alanı daraltmak/genişlemektir. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem#hideitem)(int, bool) | Bir veri alanındaki belirli PivotItem öğesinin gizli olup olmadığını ayarlar. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem#hideitem_1)(string, bool) | Bir veri alanındaki belirli PivotItem öğesinin gizli olup olmadığını ayarlar. |
| [HideItemDetail](../../aspose.cells.pivot/pivotfield/hideitemdetail)(int, bool) | Bir pivot alanındaki belirli PivotItem'in gizli ayrıntı olup olmadığını ayarlar. |
| [InitPivotItems](../../aspose.cells.pivot/pivotfield/initpivotitems)() | Özet alanının özet öğelerini başlat |
| [IsHiddenItem](../../aspose.cells.pivot/pivotfield/ishiddenitem)(int) | Belirli PivotItem'in gizli olup olmadığını gösterir. |
| [IsHiddenItemDetail](../../aspose.cells.pivot/pivotfield/ishiddenitemdetail)(int) | Belirli PivotItem'in gizli ayrıntı olup olmadığını gösterir. |
| [SetSubtotals](../../aspose.cells.pivot/pivotfield/setsubtotals)(PivotFieldSubtotalType, bool) | Belirtilen alanın bu alt toplamları gösterip göstermediğini ayarlar. |

### Örnekler

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

//PivotField'in özniteliklerini değiştir
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

pivot.RefreshData();
pivot.CalculateData();

//işini yap

book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
