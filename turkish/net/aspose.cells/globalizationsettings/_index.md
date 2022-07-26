---
title: GlobalizationSettings
second_title: Aspose.Cells for .NET API Referansı
description: Küreselleştirme ayarlarını temsil eder.
type: docs
weight: 3620
url: /tr/net/aspose.cells/globalizationsettings/
---
## GlobalizationSettings class

Küreselleştirme ayarlarını temsil eder.

```csharp
public class GlobalizationSettings : AbstractGlobalizationSettings
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [GlobalizationSettings](globalizationsettings)() | Default_Constructor |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings) { get; set; } | Bunun Grafiği'ni alır veya ayarlar[`ChartGlobalizationSettings`](../../aspose.cells.charts/chartglobalizationsettings) |
| virtual [ColumnSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/columnseparatorofformulaarray) { get; } | Formüldeki dizinin satır verilerindeki öğeler için ayırıcıyı alır. |
| virtual [ListSeparator](../../aspose.cells/globalizationsettings/listseparator) { get; } | Liste, işlev parametreleri, ...etc. için ayırıcıyı alır |
| virtual [RowSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/rowseparatorofformulaarray) { get; } | Formüldeki dizi verilerindeki satırlar için ayırıcıyı alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| virtual [Compare](../../aspose.cells/abstractglobalizationsettings/compare)(string, string, bool) | Belirli harmanlama kurallarına göre iki dize değerini karşılaştırır. |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname)() | PivotTable'da "(Tümü)" etiketinin adını alır. |
| virtual [GetBooleanValueString](../../aspose.cells/globalizationsettings/getbooleanvaluestring)(bool) | Hücrenin boole değeri için görüntülenen dize değerini alır |
| virtual [GetCollationKey](../../aspose.cells/abstractglobalizationsettings/getcollationkey)(string, bool) | Dizeyi belirli harmanlama kurallarına göre karşılaştırılabilir bir nesneye dönüştürür. |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable)() | PivotTable'da "Sütun Etiketleri" etiketinin adını alır. |
| virtual [GetCommentTitleName](../../aspose.cells/globalizationsettings/getcommenttitlename)(CommentTitleType) | Yorum başlığı türüne göre yerel ayara bağlı yorum başlığı adını alır. |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname)() | PivotTable'da "(boş)" etiketinin adını alır. |
| virtual [GetErrorValueString](../../aspose.cells/globalizationsettings/geterrorvaluestring)(string) | Hücrenin hata değeri için görüntülenen dize değerini alır |
| virtual [GetGrandTotalName](../../aspose.cells/globalizationsettings/getgrandtotalname)(ConsolidationFunction) | İşlevin genel toplam adını alır. |
| virtual [GetLocalBuiltInName](../../aspose.cells/globalizationsettings/getlocalbuiltinname)(string) | Verilen standart metne göre yerleşik Ad için yerel ayara bağlı metni alır. |
| virtual [GetLocalFunctionName](../../aspose.cells/globalizationsettings/getlocalfunctionname)(string) | Verilen standart işlev adına göre yerel ayara bağlı işlev adını alır. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname)() | PivotTable'da "(Birden Çok Öğe)" etiketinin adını alır. |
| virtual [GetOtherName](../../aspose.cells/globalizationsettings/getothername)() | Pasta grafikler için "Diğer" etiketlerin adını alır. |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname)() | PivotTable'da "Grand Total" etiketinin adını alır. |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname)() | PivotTable'da "Toplam" etiketinin adını alır. PivotTable veri alanında iki veya daha fazla PivotField içerdiğinde bu yöntemi geçersiz kılmanız gerekir. |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable)() | PivotTable'daki koruma adını alır. |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable)() | PivotTable'da "Satır Etiketleri" etiketinin adını alır. |
| virtual [GetStandardBuiltInName](../../aspose.cells/globalizationsettings/getstandardbuiltinname)(string) | Verilen yerel ayara bağlı metne göre yerleşik Ad'ın standart metnini alır. |
| virtual [GetStandardFunctionName](../../aspose.cells/globalizationsettings/getstandardfunctionname)(string) | Verilen yerel ayara bağlı işlev adına göre standart işlev adını alır. |
| virtual [GetStandardHeaderFooterFontStyleName](../../aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename)(string) | Verilen yerel yazı tipi stili adına göre Üstbilgi/Altbilgi için standart İngilizce yazı tipi stili adını (Normal, Kalın, İtalik) alır. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname)(PivotFieldSubtotalType) | Adını alır[`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype) PivotTable'ı yazın. |
| virtual [GetTableRowTypeOfAll](../../aspose.cells/globalizationsettings/gettablerowtypeofall)() | Başvurulan tablodaki tüm satırlardan oluşan tablo satırlarının tür adını alır. Varsayılan "Tümü"dür, bu nedenle "#Tümü" formülünde başvurulan tablodaki tüm satırları temsil eder. |
| virtual [GetTableRowTypeOfCurrent](../../aspose.cells/globalizationsettings/gettablerowtypeofcurrent)() | Başvurulan tablodaki geçerli satırdan oluşan tablo satırlarının tür adını alır. Varsayılan "Bu Satır"dır, dolayısıyla "#Bu Satır" formülünde başvurulan tablodaki geçerli satırı temsil eder. |
| virtual [GetTableRowTypeOfData](../../aspose.cells/globalizationsettings/gettablerowtypeofdata)() | Başvurulan tablonun veri bölgesinden oluşan tablo satırlarının tür adını alır. Varsayılan "Veri"dir, dolayısıyla "#Data" formülünde tablonun veri bölgesini temsil eder. |
| virtual [GetTableRowTypeOfHeaders](../../aspose.cells/globalizationsettings/gettablerowtypeofheaders)() | Tablo başlığından oluşan tablo satırlarının tür adını alır. Varsayılan "Başlıklar"dır, bu nedenle formülde "#Başlıklar" tablo başlığını temsil eder. |
| virtual [GetTableRowTypeOfTotals](../../aspose.cells/globalizationsettings/gettablerowtypeoftotals)() | Başvurulan tablonun toplam satırından oluşan tablo satırlarının tür adını alır. Varsayılan "Toplamlar"dır, dolayısıyla "#Toplamlar" formülünde başvurulan tablonun toplam satırını temsil eder. |
| virtual [GetTotalName](../../aspose.cells/globalizationsettings/gettotalname)(ConsolidationFunction) | İşlevin toplam adını alır. |

### Ayrıca bakınız

* class [AbstractGlobalizationSettings](../abstractglobalizationsettings)
* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
