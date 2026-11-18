---
title: "DeleteBlankOptions Class"
linktitle: "DeleteBlankOptions"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "DeleteBlankOptions class. Go'da deleteblankoptions'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/deleteblankoptions/
---

## DeleteBlankOptions class

Boş hücreleri/satırları/sütunları silme ayarını temsil eder.

```go

type DeleteBlankOptions struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewDeleteBlankOptions](./newdeleteblankoptions/) | Varsayılan yapıcı. |
| [NewDeleteBlankOptions_DeleteOptions](./newdeleteblankoptions_deleteoptions/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetEmptyStringAsBlank](./getemptystringasblank/) | Bir hücrenin değeri boş bir dize olduğunda boş olarak kabul edilip edilmeyeceğini gösterir. Varsayılan değer true'dur. |
| [SetEmptyStringAsBlank](./setemptystringasblank/) | Bir hücrenin değeri boş bir dize olduğunda boş olarak kabul edilip edilmeyeceğini gösterir. Varsayılan değer true'dur. |
| [GetEmptyFormulaValueAsBlank](./getemptyformulavalueasblank/) | Bir hücre formül olduğunda ve hesaplanan sonuç null ya da boş bir dize olduğunda boş olarak kabul edilip edilmeyeceğini gösterir. Varsayılan değer false'tur. |
| [SetEmptyFormulaValueAsBlank](./setemptyformulavalueasblank/) | Bir hücre formül olduğunda ve hesaplanan sonuç null ya da boş bir dize olduğunda boş olarak kabul edilip edilmeyeceğini gösterir. Varsayılan değer false'tur. |
| [GetDrawingsAsBlank](./getdrawingsasblank/) | Resim, şekil, grafik... gibi çizimle ilgili nesnelerin boş olarak kabul edilip edilmeyeceğini gösterir. Varsayılan değer true'dur. |
| [SetDrawingsAsBlank](./setdrawingsasblank/) | Resim, şekil, grafik... gibi çizimle ilgili nesnelerin boş olarak kabul edilip edilmeyeceğini gösterir. Varsayılan değer true'dur. |
| [GetMergedCellsShrinkType](./getmergedcellsshrinktype/) | Boş satır/sütunlar silinirken birleştirilmiş hücrelerin nasıl işleneceğini gösterir. |
| [SetMergedCellsShrinkType](./setmergedcellsshrinktype/) | Boş satır/sütunlar silinirken birleştirilmiş hücrelerin nasıl işleneceğini gösterir. |
| [GetStartIndex](./getstartindex/) | Kontrol edilecek ve boş satır/sütun silinecek aralığın başlangıç satır/sütun indeksini belirtir. |
| [SetStartIndex](./setstartindex/) | Kontrol edilecek ve boş satır/sütun silinecek aralığın başlangıç satır/sütun indeksini belirtir. |
| [GetEndIndex](./getendindex/) | Kontrol edilecek ve boş satır/sütun silinecek aralığın (dahil) son satır/sütun indeksini belirtir. Varsayılan değer -1'dir ve -1, kontrol edilmesi gereken tüm nesnelerin (hücreler, çizimler, ...) maksimum aralığını ifade eder. |
| [SetEndIndex](./setendindex/) | Kontrol edilecek ve boş satır/sütun silinecek aralığın (dahil) son satır/sütun indeksini belirtir. Varsayılan değer -1'dir ve -1, kontrol edilmesi gereken tüm nesnelerin (hücreler, çizimler, ...) maksimum aralığını ifade eder. |
| [GetUpdateReference](./getupdatereference/) | Diğer çalışma sayfalarındaki güncelleme referanslarını gösterir. |
| [SetUpdateReference](./setupdatereference/) | Diğer çalışma sayfalarındaki güncelleme referanslarını gösterir. |
| [GetFormulaChangeMonitor](./getformulachangemonitor/) | Silme nedeniyle oluşan değişiklikleri izlemek için monitörü alır/ayarlar. |
| [SetFormulaChangeMonitor](./setformulachangemonitor/) | Silme nedeniyle oluşan değişiklikleri izlemek için monitörü alır/ayarlar. |
