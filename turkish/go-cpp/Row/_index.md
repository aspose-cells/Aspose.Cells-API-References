---
title: "Row Sınıfı"
linktitle: "Row"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "Row class. Go dilinde satırı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/row/
---

## Row class

Bir çalışma sayfasındaki tek bir satırı temsil eder.

```go

type Row struct  {
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
| [GetCellByIndex](./getcellbyindex/) | Bu satırın hücre koleksiyonunda belirli bir indeksle hücreyi al. |
| [IsBlank](./isblank/) | Satırın herhangi bir veri içerip içermediğini gösterir |
| [Get](./get/) | Hücreyi alır. |
| [GetEnumerator](./getenumerator/) | Hücre enumeratörünü alır |
| [GetEnumerator_Bool_Bool](./getenumerator_bool_bool/) | Bu satırdaki hücreler üzerinde yineleme yapan bir enumeratör alır. |
| [GetCellOrNull](./getcellornull/) | Belirli indekste hücreyi veya null değerini alır. |
| [IsCollapsed](./iscollapsed/) | satırın daraltılmış olup olmadığı |
| [SetIsCollapsed](./setiscollapsed/) | satırın daraltılmış olup olmadığı |
| [GetHeight](./getheight/) | Satır yüksekliğini Point biriminde alır ve ayarlar. |
| [SetHeight](./setheight/) | Satır yüksekliğini Point biriminde alır ve ayarlar. |
| [IsHidden](./ishidden/) | Satırın gizli olup olmadığını gösterir. |
| [SetIsHidden](./setishidden/) | Satırın gizli olup olmadığını gösterir. |
| [GetIndex](./getindex/) | Bu satırın dizinini alır. |
| [GetGroupLevel](./getgrouplevel/) | Satırın grup seviyesini alır. |
| [SetGroupLevel](./setgrouplevel/) | Satırın grup seviyesini alır. |
| [IsHeightMatched](./isheightmatched/) | Satır yüksekliğinin çalışma kitabının mevcut varsayılan yazı tipi ayarına uyup uymadığını gösterir. Bu özelliğin true olması, satır yüksekliğinin kullanıcı tarafından özel bir değer ayarlanmadan "otomatik" olduğunu da gösterir. |
| [SetIsHeightMatched](./setisheightmatched/) | Satır yüksekliğinin çalışma kitabının mevcut varsayılan yazı tipi ayarına uyup uymadığını gösterir. Bu özelliğin true olması, satır yüksekliğinin kullanıcı tarafından özel bir değer ayarlanmadan "otomatik" olduğunu da gösterir. |
| [GetStyle](./getstyle/) | Bu satırın stilini alır. |
| [SetStyle](./setstyle/) | Bu satırın stilini ayarlar. |
| [GetHasCustomStyle](./gethascustomstyle/) | Bu satırın özelleştirilmiş stil ayarlarına (çalışma kitabından devralınan varsayılan stilden farklı) sahip olup olmadığını gösterir. |
| [CopySettings](./copysettings/) | Satırın ayarlarını, stil, yükseklik, görünürlük gibi, ... vb. kopyalar. |
| [GetFirstCell](./getfirstcell/) | Satırdaki ilk hücre nesnesini alır. |
| [GetFirstDataCell](./getfirstdatacell/) | Satırdaki ilk boş olmayan hücreyi alır. |
| [GetLastCell](./getlastcell/) | Satırdaki son hücre nesnesini alır. |
| [GetLastDataCell](./getlastdatacell/) | Satırdaki son boş olmayan hücreyi alır. |
| [ApplyStyle](./applystyle/) | Bir bütün satır için biçimleri uygular. |
| [Equals_Object](./equals_object/) | Bu nesnenin başka bir nesneyle aynı satıra işaret edip etmediğini kontrol eder. |
| [Equals_Row](./equals_row/) | Bu nesnenin başka bir satır nesnesiyle aynı satıra işaret edip etmediğini kontrol eder. |
