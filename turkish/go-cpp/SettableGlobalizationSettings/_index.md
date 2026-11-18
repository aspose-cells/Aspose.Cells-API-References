---
title: "SettableGlobalizationSettings Sınıfı"
linktitle: "SettableGlobalizationSettings"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "SettableGlobalizationSettings sınıfı. Go'da settableglobalizationsettings'ı temsil eden nesneyi kapsar."
type: docs
weight: 200
url: /tr/go-cpp/settableglobalizationsettings/
---

## SettableGlobalizationSettings class

Kullanıcının önceden tanımlı metinleri ayarlamasına/değiştirmesine olanak tanıyan GlobalizationSettings uygulaması.

```go

type SettableGlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewSettableGlobalizationSettings](./newsettableglobalizationsettings/) | Varsayılan yapıcı. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetTotalName](./gettotalname/) | Belirli işlevin toplam adını alır. |
| [SetTotalName](./settotalname/) | Belirli işlevin toplam adını ayarlar. |
| [GetGrandTotalName](./getgrandtotalname/) | Fonksiyonun genel toplam adını alır. |
| [SetGrandTotalName](./setgrandtotalname/) | Belirli bir fonksiyonun genel toplam adını ayarlar. |
| [GetTableRowTypeOfHeaders](./gettablerowtypeofheaders/) | Tablo başlığından oluşan tablo satırlarının tip adını alır. Varsayılan "Headers"dır, bu yüzden formülde "#Headers" tablo başlığını temsil eder. |
| [SetTableRowTypeOfHeaders](./settablerowtypeofheaders/) | Tablo başlığından oluşan tablo satırlarının tip adını ayarlar. |
| [GetTableRowTypeOfData](./gettablerowtypeofdata/) | Referans alınan tablonun veri bölgesinden oluşan tablo satırlarının tip adını alır. Varsayılan "Data"dır, bu yüzden formülde "#Data" tablonun veri bölgesini temsil eder. |
| [SetTableRowTypeOfData](./settablerowtypeofdata/) | Referans alınan tablonun veri bölgesinden oluşan tablo satırlarının tip adını ayarlar. |
| [GetTableRowTypeOfAll](./gettablerowtypeofall/) | Referans alınan tablodaki tüm satırlardan oluşan tablo satırlarının tip adını alır. |
| [SetTableRowTypeOfAll](./settablerowtypeofall/) | Referans alınan tablodaki tüm satırlardan oluşan tablo satırlarının tip adını ayarlar. |
| [GetTableRowTypeOfTotals](./gettablerowtypeoftotals/) | Referans alınan tablonun toplam satırından oluşan tablo satırlarının tip adını alır. |
| [SetTableRowTypeOfTotals](./settablerowtypeoftotals/) | Referans alınan tablonun toplam satırından oluşan tablo satırlarının tip adını ayarlar. |
| [GetTableRowTypeOfCurrent](./gettablerowtypeofcurrent/) | Referans alınan tablodaki mevcut satırdan oluşan tablo satırlarının tip adını alır. |
| [SetTableRowTypeOfCurrent](./settablerowtypeofcurrent/) | Referans alınan tablodaki mevcut satırdan oluşan tablo satırlarının tip adını ayarlar. |
| [GetErrorValueString](./geterrorvaluestring/) | Hücrenin hata değeri için görüntüleme dizesi değerini alır |
| [GetBooleanValueString](./getbooleanvaluestring/) | Hücrenin boolean değerı için görüntüleme dizesi değerini alır |
| [SetBooleanValueString](./setbooleanvaluestring/) | Hücrenin boolean değeri için görüntüleme dizesi değerini ayarlar |
| [GetLocalFunctionName](./getlocalfunctionname/) | Verilen standart fonksiyon adına göre yerel ayara bağlı fonksiyon adını alır. |
| [SetLocalFunctionName](./setlocalfunctionname/) | Verilen standart fonksiyon adına karşılık gelen yerel ayara bağlı fonksiyon adını ayarlar. |
| [GetStandardFunctionName](./getstandardfunctionname/) | Verilen yerel ayara bağlı fonksiyon adına göre standart fonksiyon adını alır. |
| [SetStandardFunctionName](./setstandardfunctionname/) | Verilen standart fonksiyon adına göre yerel ayara bağlı fonksiyon adını ayarlar. |
| [GetLocalBuiltInName](./getlocalbuiltinname/) | Verilen standart metne göre yerel ayara bağlı yerleşik Ad için metni alır. |
| [SetLocalBuiltInName](./setlocalbuiltinname/) | Verilen standart ad metniyle yerleşik ad için yerel ayara bağlı metni ayarlar. |
| [GetStandardBuiltInName](./getstandardbuiltinname/) | Verilen yerel ayara bağlı metne göre yerleşik Adın standart metnini alır. |
| [SetStandardBuiltInName](./setstandardbuiltinname/) | Verilen standart fonksiyon adına göre yerel ayara bağlı fonksiyon adını ayarlar. |
| [GetListSeparator](./getlistseparator/) | Liste, fonksiyon parametreleri vb. için ayırıcıyı alır. |
| [SetListSeparator](./setlistseparator/) | Liste, fonksiyon parametreleri vb. için ayırıcıyı ayarlar. |
| [GetRowSeparatorOfFormulaArray](./getrowseparatorofformulaarray/) | Formülde dizi verisindeki satırlar için ayırıcıyı alır. |
| [SetRowSeparatorOfFormulaArray](./setrowseparatorofformulaarray/) | Formülde dizi verilerindeki satırlar için ayırıcıyı ayarlar. |
| [GetColumnSeparatorOfFormulaArray](./getcolumnseparatorofformulaarray/) | Formülde dizi satır verilerindeki öğeler için ayırıcıyı alır. |
| [SetColumnSeparatorOfFormulaArray](./setcolumnseparatorofformulaarray/) | Formülde dizi satır verilerindeki öğeler için ayırıcıyı ayarlar. |
| [GetStandardHeaderFooterFontStyleName](./getstandardheaderfooterfontstylename/) | Verilen yerel yazı tipi stil adına göre Üstbilgi/Altbilgi için standart İngilizce yazı tipi stil adını (Regular, Bold, Italic) alır. |
| [SetStandardHeaderFooterFontStyleName](./setstandardheaderfooterfontstylename/) | Verilen standart fonksiyon adına göre yerel ayara bağlı fonksiyon adını ayarlar. |
| [GetCommentTitleName](./getcommenttitlename/) | Yorum başlığı türüne göre yerel bağımlı yorum başlığı adını alır. |
| [SetCommentTitleName](./setcommenttitlename/) | Yorum başlığı türüne göre yerel bağımlı yorum başlığı adını alır. |
