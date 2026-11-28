---
title: "Sınıf SettableGlobalizationSettings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.SettableGlobalizationSettings sınıfı. Kullanıcıların önceden tanımlı metinleri ayarlamasını/değiştirmesini destekleyen GlobalizationSettings'in uygulanması"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/
---
## SettableGlobalizationSettings class

Kullanıcının önceden tanımlı metinleri ayarlamasına/değiştirmesine olanak tanıyan GlobalizationSettings uygulaması.

```csharp
public class SettableGlobalizationSettings : GlobalizationSettings
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [SettableGlobalizationSettings](settableglobalizationsettings/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings/) { get; set; } | Grafik için küreselleştirme ayarlarını alır veya ayarlar. ([`GlobalizationSettings`](../globalizationsettings/) üzerinden devralınmıştır.) |
| override [ColumnSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/columnseparatorofformulaarray/) { get; } | Formülde dizi satır verilerindeki öğeler için ayırıcıyı alır. |
| override [ListSeparator](../../aspose.cells/settableglobalizationsettings/listseparator/) { get; } | Liste, fonksiyon parametreleri, ... vb. için ayırıcıyı alır. |
| [PivotSettings](../../aspose.cells/globalizationsettings/pivotsettings/) { get; set; } | Özet tablo için küreselleştirme ayarlarını alır veya ayarlar. ([`GlobalizationSettings`](../globalizationsettings/) üzerinden devralınmıştır.) |
| override [RowSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/rowseparatorofformulaarray/) { get; } | Formülde dizi verilerindeki satırlar için ayırıcıyı alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| virtual [Compare](../../aspose.cells/globalizationsettings/compare/)(string, string, bool) | Belirli sıralama kurallarına göre iki dize değerini karşılaştırır. ([`GlobalizationSettings`](../globalizationsettings/) üzerinden devralınmıştır.) |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname/)() | (**Eski.**) PivotTable içinde "(All)" etiketinin adını alır. (Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetBooleanValueString](../../aspose.cells/settableglobalizationsettings/getbooleanvaluestring/)(bool) | Hücrenin boolean değerinin görüntüleme dizesi değerini alır |
| virtual [GetCollationKey](../../aspose.cells/globalizationsettings/getcollationkey/)(string, bool) | Dizgiyi belirli sıralama kurallarına göre karşılaştırılabilir bir nesneye dönüştürür. (Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/)() | (**Eski.**) PivotTable içinde "Column Labels" etiketinin adını alır. (Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetCommentTitleName](../../aspose.cells/settableglobalizationsettings/getcommenttitlename/)(CommentTitleType) | Yorum başlığı türüne göre yerel ayara bağlı yorum başlığı adını alır. |
| virtual [GetDataFieldHeaderNameOfPivotTable](../../aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/)() | (**Eski.**) PivotTable içinde değer alanı alan başlığının adını alır. (Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetDefaultSheetName](../../aspose.cells/globalizationsettings/getdefaultsheetname/)() | Çalışma sayfası eklemek için varsayılan sayfa adını alır. Varsayılan "Sheet". (Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname/)() | (**Eski.**) PivotTable içinde "(blank)" etiketinin adını alır. (Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetErrorValueString](../../aspose.cells/settableglobalizationsettings/geterrorvaluestring/)(string) | Hücrenin hata değerinin görüntüleme dizesi değerini alır |
| override [GetGrandTotalName](../../aspose.cells/settableglobalizationsettings/getgrandtotalname/)(ConsolidationFunction) | Fonksiyonun genel toplam adını alır. |
| override [GetLocalBuiltInName](../../aspose.cells/settableglobalizationsettings/getlocalbuiltinname/)(string) | Verilen standart metne göre yerel ayara bağlı yerleşik Name metnini alır. |
| override [GetLocalFunctionName](../../aspose.cells/settableglobalizationsettings/getlocalfunctionname/)(string) | Verilen standart fonksiyon adına göre yerel ayara bağlı fonksiyon adını alır. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname/)() | (**Eski.**) PivotTable içinde "(Multiple Items)" etiketinin adını alır. (Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname/)() | (**Eski.**) PivotTable içinde "Grand Total" etiketinin adını alır. (Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname/)() | (**Eski.**) PivotTable içinde "Total" etiketinin adını alır. PivotTable veri alanında iki veya daha fazla PivotField içerdiğinde bu yöntemi geçersiz kılmanız gerekir. (Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable/)() | (**Eski.**) PivotTable içindeki koruma adını alır. (Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/)() | (**Eski.**) PivotTable içinde "Row Labels" etiketinin adını alır. (Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetStandardBuiltInName](../../aspose.cells/settableglobalizationsettings/getstandardbuiltinname/)(string) | Verilen yerel ayara bağlı metne göre yerleşik Name'in standart metnini alır. |
| override [GetStandardFunctionName](../../aspose.cells/settableglobalizationsettings/getstandardfunctionname/)(string) | Verilen yerel ayara bağlı fonksiyon adına göre standart fonksiyon adını alır. |
| override [GetStandardHeaderFooterFontStyleName](../../aspose.cells/settableglobalizationsettings/getstandardheaderfooterfontstylename/)(string) | Verilen yerel font stiline göre Başlık/Altbilgi için standart İngilizce yazı tipi stil adını (Regular, Bold, Italic) alır. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname/)(PivotFieldSubtotalType) | (**Eski.**) PivotTable içinde [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) tipinin adını alır. (Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetTableRowTypeOfAll](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofall/)() | Referans verilen tabloda tüm satırları içeren tablo satırlarının tip adını alır. |
| override [GetTableRowTypeOfCurrent](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofcurrent/)() | Referans verilen tabloda mevcut satırı içeren tablo satırlarının tip adını alır. |
| override [GetTableRowTypeOfData](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofdata/)() | Referans verilen tablonun veri bölgesini içeren tablo satırlarının tip adını alır. Varsayılan "Data"dır, bu yüzden formülde "#Data" tabloyun veri bölgesini temsil eder. |
| override [GetTableRowTypeOfHeaders](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofheaders/)() | Tablo başlığını içeren tablo satırlarının tip adını alır. Varsayılan "Headers"dır, bu yüzden formülde "#Headers" tablo başlığını temsil eder. |
| override [GetTableRowTypeOfTotals](../../aspose.cells/settableglobalizationsettings/gettablerowtypeoftotals/)() | Referans alınan tablonun toplam satırını içeren tablo satırlarının tür adını alır. |
| override [GetTotalName](../../aspose.cells/settableglobalizationsettings/gettotalname/)(ConsolidationFunction) | Belirli işlevin toplam adını alır. |
| [SetBooleanValueString](../../aspose.cells/settableglobalizationsettings/setbooleanvaluestring/)(bool, string) | Hücrenin boolean değerinin görüntüleme dizesi değerini ayarlar |
| [SetColumnSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/setcolumnseparatorofformulaarray/)(char) | Formülde dizinin satır verisindeki öğeler için ayırıcıyı ayarlar. |
| [SetCommentTitleName](../../aspose.cells/settableglobalizationsettings/setcommenttitlename/)(CommentTitleType, string) | Yorum başlığı türüne göre yerel ayara bağlı yorum başlığı adını alır. |
| [SetGrandTotalName](../../aspose.cells/settableglobalizationsettings/setgrandtotalname/)(ConsolidationFunction, string) | Belirli işlevin genel toplam adını ayarlar. |
| [SetListSeparator](../../aspose.cells/settableglobalizationsettings/setlistseparator/)(char) | Liste, işlev parametreleri vb. için ayırıcıyı ayarlar. |
| [SetLocalBuiltInName](../../aspose.cells/settableglobalizationsettings/setlocalbuiltinname/)(string, string, bool) | Verilen standart ad metniyle yerleşik ad için yerel bağımlı metni ayarlar. |
| [SetLocalFunctionName](../../aspose.cells/settableglobalizationsettings/setlocalfunctionname/)(string, string, bool) | Verilen standart işlev adına karşılık gelen yerel bağımlı işlev adını ayarlar. |
| [SetRowSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/setrowseparatorofformulaarray/)(char) | Formülde dizi verisindeki satırlar için ayırıcıyı ayarlar. |
| [SetStandardBuiltInName](../../aspose.cells/settableglobalizationsettings/setstandardbuiltinname/)(string, string, bool) | Verilen standart işlev adına göre yerel bağımlı işlev adını ayarlar. |
| [SetStandardFunctionName](../../aspose.cells/settableglobalizationsettings/setstandardfunctionname/)(string, string, bool) | Verilen standart işlev adına göre yerel bağımlı işlev adını ayarlar. |
| [SetStandardHeaderFooterFontStyleName](../../aspose.cells/settableglobalizationsettings/setstandardheaderfooterfontstylename/)(string, string) | Verilen standart işlev adına göre yerel bağımlı işlev adını ayarlar. |
| [SetTableRowTypeOfAll](../../aspose.cells/settableglobalizationsettings/settablerowtypeofall/)(string) | Referans alınan tablodaki tüm satırları içeren tablo satırlarının tür adını ayarlar. |
| [SetTableRowTypeOfCurrent](../../aspose.cells/settableglobalizationsettings/settablerowtypeofcurrent/)(string) | Referans alınan tablodaki mevcut satırı içeren tablo satırlarının tür adını ayarlar. |
| [SetTableRowTypeOfData](../../aspose.cells/settableglobalizationsettings/settablerowtypeofdata/)(string) | Referans alınan tablonun veri bölgesini içeren tablo satırlarının tür adını ayarlar. |
| [SetTableRowTypeOfHeaders](../../aspose.cells/settableglobalizationsettings/settablerowtypeofheaders/)(string) | Tablo başlığını içeren tablo satırlarının tür adını ayarlar. |
| [SetTableRowTypeOfTotals](../../aspose.cells/settableglobalizationsettings/settablerowtypeoftotals/)(string) | Referans alınan tablonun toplam satırını içeren tablo satırlarının tür adını ayarlar. |
| [SetTotalName](../../aspose.cells/settableglobalizationsettings/settotalname/)(ConsolidationFunction, string) | Belirli işlevin toplam adını ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;

    public class CellsClassSettableGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // SettableGlobalizationSettings örneği oluştur
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // Özel liste ayırıcıyı ayarla
            settings.SetListSeparator(';');

            // Özel boolean değer dizesini ayarla
            settings.SetBooleanValueString(true, "TRUE_CUSTOM");
            settings.SetBooleanValueString(false, "FALSE_CUSTOM");

            // Özel işlev adlarını ayarla
            settings.SetLocalFunctionName("SUM", "SUMME", true);
            settings.SetLocalFunctionName("AVERAGE", "MITTELWERT", true);

            // Özel tablo satırı tür adlarını ayarla
            settings.SetTableRowTypeOfHeaders("HEADERS_CUSTOM");
            settings.SetTableRowTypeOfData("DATA_CUSTOM");
            settings.SetTableRowTypeOfTotals("TOTALS_CUSTOM");

            // Özel yorum başlığı adlarını ayarla
            settings.SetCommentTitleName(CommentTitleType.Comment, "COMMENT_CUSTOM");
            // CommentTitleType'ın o enum değerine sahip olmaması nedeniyle Yazar satırı kaldırıldı
            // Yazarla ilgili ayarları ayarlamanız gerekiyorsa, bunun yerine ThreadedCommentAuthor kullanmanız gerekir

            // Küreselleştirme ayarlarını çalışma kitabına uygula
            workbook.Settings.GlobalizationSettings = settings;

            // Formüllerde kullanımı göster
            worksheet.Cells["A1"].Formula = "=TRUE()";
            worksheet.Cells["A2"].Formula = "=FALSE()";
            worksheet.Cells["A3"].Formula = "=SUM(1,2,3)";
            worksheet.Cells["A4"].Formula = "=AVERAGE(1,2,3)";

            // Çalışma kitabını kaydedin
            workbook.Save("SettableGlobalizationSettingsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [GlobalizationSettings](../globalizationsettings/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


