---
title: "ImportTableOptions Sınıfı"
linktitle: "ImportTableOptions"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "ImportTableOptions sınıf. Go'da importtableoptions'ı temsil eden nesneyi kapsar."
type: docs
weight: 200
url: /tr/go-cpp/importtableoptions/
---

## ImportTableOptions class

Verilerin hücrelere içe aktarılması seçeneklerini temsil eder.

```go

type ImportTableOptions struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewImportTableOptions](./newimporttableoptions/) | Varsayılan içe aktarma seçeneklerini oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetConvertGridStyle](./getconvertgridstyle/) | Izgara görünümünün stilini hücrelere uygulayıp uygulamayacağını gösterir. |
| [SetConvertGridStyle](./setconvertgridstyle/) | Izgara görünümünün stilini hücrelere uygulayıp uygulamayacağını gösterir. |
| [GetConvertNumericData](./getconvertnumericdata/) | Dize değerinin sayısal veya tarih değerine dönüştürülüp dönüştürülmeyeceğini gösteren bir değeri alır veya ayarlar. |
| [SetConvertNumericData](./setconvertnumericdata/) | Dize değerinin sayısal veya tarih değerine dönüştürülüp dönüştürülmeyeceğini gösteren bir değeri alır veya ayarlar. |
| [GetInsertRows](./getinsertrows/) | Veri kayıtlarını içe aktarmak için yeni satırların eklenip eklenmeyeceğini gösterir. |
| [SetInsertRows](./setinsertrows/) | Veri kayıtlarını içe aktarmak için yeni satırların eklenip eklenmeyeceğini gösterir. |
| [GetShiftFirstRowDown](./getshiftfirstrowdown/) | Satır eklerken ilk satırın aşağı kaydırılıp kaydırılmayacağını gösterir. |
| [SetShiftFirstRowDown](./setshiftfirstrowdown/) | Satır eklerken ilk satırın aşağı kaydırılıp kaydırılmayacağını gösterir. |
| [IsFieldNameShown](./isfieldnameshown/) | Alan adının içe aktarılıp aktarılmayacağını gösterir. |
| [SetIsFieldNameShown](./setisfieldnameshown/) | Alan adının içe aktarılıp aktarılmayacağını gösterir. |
| [GetExportCaptionAsFieldName](./getexportcaptionasfieldname/) | Altyazının alan adı olarak dışa aktarılıp aktarılmayacağını gösterir. |
| [SetExportCaptionAsFieldName](./setexportcaptionasfieldname/) | Altyazının alan adı olarak dışa aktarılıp aktarılmayacağını gösterir. |
| [GetDateFormat](./getdateformat/) | İçe aktarılan tarih‑zaman değerlerine sahip hücreler için tarih biçimi dizesini alır veya ayarlar. |
| [SetDateFormat](./setdateformat/) | İçe aktarılan tarih‑zaman değerlerine sahip hücreler için tarih biçimi dizesini alır veya ayarlar. |
| [GetNumberFormats](./getnumberformats/) | Sayı biçimlerini alır veya ayarlar. |
| [SetNumberFormats](./setnumberformats/) | Sayı biçimlerini alır veya ayarlar. |
| [GetStyles](./getstyles/) | Tablonun her sütunu için stilleri alır ve ayarlar. |
| [SetStyles](./setstyles/) | Tablonun her sütunu için stilleri alır ve ayarlar. |
| [GetIsFormulas](./getisformulas/) | Verilerin formül olup olmadığını gösterir. |
| [SetIsFormulas](./setisformulas/) | Verilerin formül olup olmadığını gösterir. |
| [GetTotalRows](./gettotalrows/) | Veri kaynağından içe aktarılacak toplam satır sayısını alır veya ayarlar. -1, verilen veri kaynağının tüm satırları anlamına gelir. |
| [SetTotalRows](./settotalrows/) | Veri kaynağından içe aktarılacak toplam satır sayısını alır veya ayarlar. -1, verilen veri kaynağının tüm satırları anlamına gelir. |
| [GetTotalColumns](./gettotalcolumns/) | Veri kaynağından içe aktarılacak toplam sütun sayısını alır veya ayarlar. -1, verilen veri kaynağının tüm sütunları anlamına gelir. |
| [SetTotalColumns](./settotalcolumns/) | Veri kaynağından içe aktarılacak toplam sütun sayısını alır veya ayarlar. -1, verilen veri kaynağının tüm sütunları anlamına gelir. |
| [GetColumnIndexes](./getcolumnindexes/) | Veri kaynağından içe aktarılacak sütunları (0‑tabanlı) alır veya ayarlar. null, tüm sütunların içe aktarılması gerektiğini gösterir. |
| [SetColumnIndexes](./setcolumnindexes/) | Veri kaynağından içe aktarılacak sütunları (0‑tabanlı) alır veya ayarlar. null, tüm sütunların içe aktarılması gerektiğini gösterir. |
| [GetDefaultValues](./getdefaultvalues/) | Tablodaki değerin varsayılan değeri null'dur. |
| [SetDefaultValues](./setdefaultvalues/) | Tablodaki değerin varsayılan değeri null'dur. |
| [IsHtmlString](./ishtmlstring/) | Değerin html etiketleri içerip içermediğini gösterir. |
| [SetIsHtmlString](./setishtmlstring/) | Değerin html etiketleri içerip içermediğini gösterir. |
| [GetCheckMergedCells](./getcheckmergedcells/) | Birleştirilmiş hücrelerin kontrol edilip edilmediğini gösterir. |
| [SetCheckMergedCells](./setcheckmergedcells/) | Birleştirilmiş hücrelerin kontrol edilip edilmediğini gösterir. |
