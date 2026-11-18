---
title: "GlobalizationSettings Sınıfı"
linktitle: "GlobalizationSettings"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "GlobalizationSettings sınıfı. Go'da globalizationsettings'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/globalizationsettings/
---

## GlobalizationSettings class

Küreselleştirme ayarlarını temsil eder.

```go

type GlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewGlobalizationSettings](./newglobalizationsettings/) | Varsayılan yapıcı. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetChartSettings](./getchartsettings/) | Grafik için küreselleştirme ayarlarını alır. |
| [SetChartSettings](./setchartsettings/) | Grafik için küreselleştirme ayarlarını ayarlar. |
| [GetPivotSettings](./getpivotsettings/) | Pivot tablo için küreselleştirme ayarlarını alır. |
| [SetPivotSettings](./setpivotsettings/) | Pivot tablo için küreselleştirme ayarlarını ayarlar. |
| [GetTotalName](./gettotalname/) | Fonksiyonun toplam adını alır. |
| [GetGrandTotalName](./getgrandtotalname/) | Fonksiyonun genel toplam adını alır. |
| [GetDefaultSheetName](./getdefaultsheetname/) | Çalışma sayfası eklemek için varsayılan sayfa adını otomatik alır. Varsayılan "Sheet". |
| [GetTableRowTypeOfHeaders](./gettablerowtypeofheaders/) | Tablo başlığından oluşan tablo satırlarının tip adını alır. Varsayılan "Headers"dır, bu yüzden formülde "#Headers" tablo başlığını temsil eder. |
| [GetTableRowTypeOfData](./gettablerowtypeofdata/) | Referans alınan tablonun veri bölgesinden oluşan tablo satırlarının tip adını alır. Varsayılan "Data"dır, bu yüzden formülde "#Data" tablonun veri bölgesini temsil eder. |
| [GetTableRowTypeOfAll](./gettablerowtypeofall/) | Referans alınan tabloda bulunan tüm satırları içeren tablo satırlarının tip adını alır. Varsayılan "All"'dır, bu yüzden formülde "#All" referans tablodaki tüm satırları temsil eder. |
| [GetTableRowTypeOfTotals](./gettablerowtypeoftotals/) | Referans alınan tablonun toplam satırını içeren tablo satırlarının tip adını alır. Varsayılan "Totals"'dır, bu yüzden formülde "#Totals" referans tablonun toplam satırını temsil eder. |
| [GetTableRowTypeOfCurrent](./gettablerowtypeofcurrent/) | Referans alınan tablodaki mevcut satırı içeren tablo satırlarının tip adını alır. Varsayılan "This Row"'dır, bu yüzden formülde "#This Row" referans tablodaki mevcut satırı temsil eder. |
| [GetErrorValueString](./geterrorvaluestring/) | Hücrenin hata değeri için görüntüleme dizesi değerini alır |
| [GetBooleanValueString](./getbooleanvaluestring/) | Hücrenin boolean değerı için görüntüleme dizesi değerini alır |
| [GetLocalFunctionName](./getlocalfunctionname/) | Verilen standart fonksiyon adına göre yerel ayara bağlı fonksiyon adını alır. |
| [GetStandardFunctionName](./getstandardfunctionname/) | Verilen yerel ayara bağlı fonksiyon adına göre standart fonksiyon adını alır. |
| [GetLocalBuiltInName](./getlocalbuiltinname/) | Verilen standart metne göre yerel ayara bağlı yerleşik Ad için metni alır. |
| [GetStandardBuiltInName](./getstandardbuiltinname/) | Verilen yerel ayara bağlı metne göre yerleşik Adın standart metnini alır. |
| [GetListSeparator](./getlistseparator/) | Liste, fonksiyon parametreleri vb. için ayırıcıyı alır. |
| [GetRowSeparatorOfFormulaArray](./getrowseparatorofformulaarray/) | Formülde dizi verisindeki satırlar için ayırıcıyı alır. |
| [GetColumnSeparatorOfFormulaArray](./getcolumnseparatorofformulaarray/) | Formülde dizi satır verilerindeki öğeler için ayırıcıyı alır. |
| [GetStandardHeaderFooterFontStyleName](./getstandardheaderfooterfontstylename/) | Verilen yerel yazı tipi stil adına göre Üstbilgi/Altbilgi için standart İngilizce yazı tipi stil adını (Regular, Bold, Italic) alır. |
| [GetCommentTitleName](./getcommenttitlename/) | Yorum başlığı türüne göre yerel bağımlı yorum başlığı adını alır. |
| [Compare](./compare/) | Belirli sıralama kurallarına göre iki dize değerini karşılaştırır. |
