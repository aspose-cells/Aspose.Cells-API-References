---
title: "ListObject Class"
linktitle: "ListObject"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "ListObject class. Go dilinde listobject'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/listobject/
---

## ListObject class

Bir çalışma sayfasındaki bir tabloyu temsil eder.

```go

type ListObject struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetStartRow](./getstartrow/) | Aralığın başlangıç satırını alır. |
| [GetStartColumn](./getstartcolumn/) | Aralığın başlangıç sütununu alır. |
| [GetEndRow](./getendrow/) | Aralığın son satırını alır. |
| [GetEndColumn](./getendcolumn/) | Aralığın son sütununu alır. |
| [GetListColumns](./getlistcolumns/) | Bu tablonun ListColumn listesini alır. |
| [Resize](./resize/) | Liste nesnesinin aralığını yeniden boyutlandır. |
| [PutCellValue_Int_Int_Object](./putcellvalue_int_int_object/) | Değeri hücreye yerleştir. |
| [PutCellValue_Int_Int_Object_Bool](./putcellvalue_int_int_object_bool/) | Değeri hücreye yerleştir. |
| [PutCellFormula_Int_Int_String](./putcellformula_int_int_string/) | Formülü tablodaki hücreye yerleştir. |
| [PutCellFormula_Int_Int_String_Bool](./putcellformula_int_int_string_bool/) | Formülü tablodaki hücreye yerleştir. |
| [GetShowHeaderRow](./getshowheaderrow/) | Bu Tablonun başlık satırını gösterip göstermediğini alır ve ayarlar. |
| [SetShowHeaderRow](./setshowheaderrow/) | Bu Tablonun başlık satırını gösterip göstermediğini alır ve ayarlar. |
| [GetShowTotals](./getshowtotals/) | Bu Tablonun toplam satırını gösterip göstermediğini alır ve ayarlar. |
| [SetShowTotals](./setshowtotals/) | Bu Tablonun toplam satırını gösterip göstermediğini alır ve ayarlar. |
| [GetDataRange](./getdatarange/) | Tablonun veri aralığını alır. |
| [UpdateColumnName](./updatecolumnname/) | Tüm liste sütunlarının adını tablodaki hücrelere günceller. |
| [GetQueryTable](./getquerytable/) | Bağlantılı QueryTable'ı alır. |
| [GetDataSourceType](./getdatasourcetype/) | Tablonun veri kaynağı türünü alır. |
| [GetHasAutoFilter](./gethasautofilter/) | Bu tabloya otomatik filtre uygulanıp uygulanmadığını gösterir. |
| [SetHasAutoFilter](./sethasautofilter/) | Bu tabloya otomatik filtre uygulanıp uygulanmadığını gösterir. |
| [RemoveAutoFilter](./removeautofilter/) | Bu tabloya uygulanan otomatik filtreyi kaldırır. |
| [GetAutoFilter](./getautofilter/) | Bu tablonun otomatik filtresini alır. |
| [GetDisplayName](./getdisplayname/) | Tablonun görüntüleme adını alır ve ayarlar. |
| [SetDisplayName](./setdisplayname/) | Tablonun görüntüleme adını alır ve ayarlar. |
| [GetComment](./getcomment/) | Tablonun yorumunu alır ve ayarlar. |
| [SetComment](./setcomment/) | Tablonun yorumunu alır ve ayarlar. |
| [GetShowTableStyleFirstColumn](./getshowtablestylefirstcolumn/) | Tablodaki ilk sütunun stilin uygulandığını gösterir. |
| [SetShowTableStyleFirstColumn](./setshowtablestylefirstcolumn/) | Tablodaki ilk sütunun stilin uygulandığını gösterir. |
| [GetShowTableStyleLastColumn](./getshowtablestylelastcolumn/) | Tablodaki son sütunun stilin uygulandığını gösterir. |
| [SetShowTableStyleLastColumn](./setshowtablestylelastcolumn/) | Tablodaki son sütunun stilin uygulandığını gösterir. |
| [GetShowTableStyleRowStripes](./getshowtablestylerowstripes/) | Satır şerit biçiminin uygulanıp uygulanmadığını gösterir. |
| [SetShowTableStyleRowStripes](./setshowtablestylerowstripes/) | Satır şerit biçiminin uygulanıp uygulanmadığını gösterir. |
| [GetShowTableStyleColumnStripes](./getshowtablestylecolumnstripes/) | Sütun şerit biçiminin uygulanıp uygulanmadığını gösterir. |
| [SetShowTableStyleColumnStripes](./setshowtablestylecolumnstripes/) | Sütun şerit biçiminin uygulanıp uygulanmadığını gösterir. |
| [ApplyStyleToRange](./applystyletorange/) | Tablo stilini aralığa uygula. |
| [ConvertToRange](./converttorange/) | Tabloyu aralığa dönüştür. |
| [ConvertToRange_TableToRangeOptions](./converttorange_tabletorangeoptions/) | Tabloyu aralığa dönüştür. |
| [GetTableStyleType](./gettablestyletype/) | Yerleşik tablo stilini alır. |
| [SetTableStyleType](./settablestyletype/) | Yerleşik tablo stilini alır. |
| [GetTableStyleName](./gettablestylename/) | Tablo stilinin adını alır ve ayarlar. |
| [SetTableStyleName](./settablestylename/) | Tablo stilinin adını alır ve ayarlar. |
| [GetXmlMap](./getxmlmap/) | Bu liste için kullanılan bir XmlMap'i alır. |
| [GetAlternativeText](./getalternativetext/) | Alternatif metni alır ve ayarlar. |
| [SetAlternativeText](./setalternativetext/) | Alternatif metni alır ve ayarlar. |
| [GetAlternativeDescription](./getalternativedescription/) | Alternatif açıklamayı alır ve ayarlar. |
| [SetAlternativeDescription](./setalternativedescription/) | Alternatif açıklamayı alır ve ayarlar. |
