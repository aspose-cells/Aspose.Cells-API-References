---
title: "UnionRange Sınıfı"
linktitle: "UnionRange"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "UnionRange sınıfı. Go'da unionrange'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/unionrange/
---

## UnionRange class

Birleşik aralığı temsil eder.

```go

type UnionRange struct  {
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
| [GetFirstRow](./getfirstrow/) | Aralığın ilk satırının indeksini alır. |
| [GetFirstColumn](./getfirstcolumn/) | Aralığın ilk sütununun indeksini alır. |
| [GetRowCount](./getrowcount/) | Aralıktaki satır sayısını alır. |
| [GetColumnCount](./getcolumncount/) | Aralıktaki satır sayısını alır. |
| [Merge](./merge/) | Bir hücre aralığını tek bir hücreye birleştirir. |
| [UnMerge](./unmerge/) | Bu aralıktaki birleştirilmiş hücrelerin birleştirmesini kaldırır. |
| [PutValue](./putvalue/) | Bir değeri aralığa yerleştirir, uygun olduğunda değer başka bir veri tipine dönüştürülür ve hücrenin sayı biçimi sıfırlanır. |
| [GetValue](./getvalue/) | Aralığın değerlerini alır ve ayarlar. |
| [SetValue](./setvalue/) | Aralığın değerlerini alır ve ayarlar. |
| [GetName](./getname/) | Aralığın adını alır veya ayarlar. |
| [SetName](./setname/) | Aralığın adını alır veya ayarlar. |
| [GetRefersTo](./getrefersto/) | Aralığın referansını alır. |
| [GetHasRange](./gethasrange/) | Bunun bir aralığı olup olmadığını gösterir. |
| [GetHyperlinks](./gethyperlinks/) | Aralıktaki tüm hiperbağlantıları alır. |
| [SetStyle](./setstyle/) | Aralığın stilini ayarlar. |
| [ApplyStyle](./applystyle/) | Tüm bir aralık için biçimleri uygular. |
| [Copy](./copy/) | Aralığı yapıştırma özel seçenekleriyle kopyalıyor. |
| [GetEnumerator](./getenumerator/) | Bu Range içindeki hücreler için yineleyiciyi alır. |
| [GetCellCount](./getcellcount/) | Aralıktaki tüm hücre sayısını alır. |
| [GetRangeCount](./getrangecount/) | Aralıkların sayısını alır. |
| [GetRanges](./getranges/) | Tüm birleşik aralıkları alır. |
| [SetOutlineBorders_CellBorderTypeArray_ColorArray](./setoutlineborders_cellbordertypearray_colorarray/) | Bir hücre aralığının etrafına dış kenar çizgilerini ayarlar. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | Aynı kenar stili ve rengi kullanarak bir hücre aralığının etrafına dış kenar çizgilerini ayarlar. |
| [Intersect_String](./intersect_string/) | Başka bir aralıkla kesişir. |
| [Intersect_UnionRange](./intersect_unionrange/) | Başka bir aralıkla kesişir. |
| [Intersect_RangeArray](./intersect_rangearray/) | Başka bir aralıkla kesişir. |
| [Union_String](./union_string/) | Başka bir aralığı birleştir. |
| [Union_UnionRange](./union_unionrange/) | Başka bir aralığı birleştir. |
| [Union_RangeArray](./union_rangearray/) | Aralıkları birleştir. |
