---
title: "Range Sınıfı"
linktitle: "Range"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "Range sınıfı. Go'da range'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/range/
---

## Range class

Bir elektronik tablo içinde hücre aralığını temsil eden nesneyi kapsüller.

```go

type Range struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewRange_CellArea_Cells](./newrange_cellarea_cells/) | Sınıf yapıcı. |
| [NewRange_Int_Int_Int_Int_Cells](./newrange_int_int_int_int_cells/) | Sınıf yapıcı. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [AutoFill_Range](./autofill_range/) | Hedef aralığı otomatik olarak doldurur. |
| [AutoFill_Range_AutoFillType](./autofill_range_autofilltype/) | Hedef aralığı otomatik olarak doldurur. |
| [GetCurrentRegion](./getcurrentregion/) | Geçerli bölgeyi temsil eden bir Range nesnesi döndürür. Geçerli bölge, boş satırların ve boş sütunların herhangi bir kombinasyonu ile sınırlanan bir aralıktır. |
| [GetHyperlinks](./gethyperlinks/) | Aralıktaki tüm hiperbağlantıları alır. |
| [AddHyperlink](./addhyperlink/) | Belirtilen bir hücreye veya hücre aralığına bir hiperbağlantı ekler. |
| [GetEnumerator](./getenumerator/) | Bu Range içindeki hücreler için yineleyiciyi alır. |
| [IsIntersect](./isintersect/) | Aralığın kesişip kesişmediğini belirtir. |
| [Intersect](./intersect/) | İki aralığın dikdörtgen kesişimini temsil eden bir Range nesnesi döndürür. |
| [UnionRanges](./unionranges/) | İki aralığın birleşim sonucunu döndürür. |
| [GetRowCount](./getrowcount/) | Aralıktaki satır sayısını alır. |
| [GetColumnCount](./getcolumncount/) | Aralıktaki sütun sayısını alır. |
| [GetName](./getname/) | Aralığın adını alır veya ayarlar. |
| [SetName](./setname/) | Aralığın adını alır veya ayarlar. |
| [GetRefersTo](./getrefersto/) | Aralığın referansını alır. |
| [GetAddress](./getaddress/) | Aralığın adresini alır. |
| [IsBlank](./isblank/) | Aralığın değer içerip içermediğini gösterir. |
| [GetLeft](./getleft/) | Aralığın sol kenarı ile A sütununun sol kenarı arasındaki mesafeyi puan cinsinden alır. |
| [GetTop](./gettop/) | Aralığın üst kenarı ile 1. satırın üst kenarı arasındaki mesafeyi puan cinsinden alır. |
| [GetWidth](./getwidth/) | Bir aralığın genişliğini puan cinsinden alır. |
| [GetHeight](./getheight/) | Bir aralığın genişliğini puan cinsinden alır. |
| [GetFirstRow](./getfirstrow/) | Aralığın ilk satırının indeksini alır. |
| [GetFirstColumn](./getfirstcolumn/) | Aralığın ilk sütununun indeksini alır. |
| [Merge](./merge/) | Bir hücre aralığını tek bir hücreye birleştirir. |
| [UnMerge](./unmerge/) | Bu aralıktaki birleştirilmiş hücrelerin birleştirmesini kaldırır. |
| [PutValue](./putvalue/) | Bir değeri aralığa yerleştirir, uygun olduğunda değer başka bir veri tipine dönüştürülür ve hücrenin sayı biçimi sıfırlanır. |
| [GetValue](./getvalue/) | Aralığın değerini alır ve ayarlar. |
| [SetValue](./setvalue/) | Aralığın değerini alır ve ayarlar. |
| [SetStyle_Style_Bool](./setstyle_style_bool/) | Hücre stilini uygula. |
| [ApplyStyle](./applystyle/) | Tüm bir aralık için biçimleri uygular. |
| [SetStyle_Style](./setstyle_style/) | Aralığın stilini ayarlar. |
| [SetOutlineBorders_CellBorderType_CellsColor](./setoutlineborders_cellbordertype_cellscolor/) | Aynı kenar stili ve rengi kullanarak bir hücre aralığının etrafına dış kenar çizgilerini ayarlar. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | Aynı kenar stili ve rengi kullanarak bir hücre aralığının etrafına dış kenar çizgilerini ayarlar. |
| [SetOutlineBorders_CellBorderTypeArray_ColorArray](./setoutlineborders_cellbordertypearray_colorarray/) | Bir hücre aralığının etrafına dış kenar çizgilerini ayarlar. |
| [SetOutlineBorder_BorderType_CellBorderType_CellsColor](./setoutlineborder_bordertype_cellbordertype_cellscolor/) | Bir hücre aralığının etrafına dış kenar çizgisi ayarlar. |
| [SetOutlineBorder_BorderType_CellBorderType_Color](./setoutlineborder_bordertype_cellbordertype_color/) | Bir hücre aralığının etrafına dış kenar çizgisi ayarlar. |
| [SetInsideBorders](./setinsideborders/) | Aralığın iç kenarlarını ayarlar. |
| [GetColumnWidth](./getcolumnwidth/) | Bu aralığın sütun genişliğini ayarlar veya alır |
| [SetColumnWidth](./setcolumnwidth/) | Bu aralığın sütun genişliğini ayarlar veya alır |
| [GetRowHeight](./getrowheight/) | Bu aralıktaki satırların yüksekliğini ayarlar veya alır |
| [SetRowHeight](./setrowheight/) | Bu aralıktaki satırların yüksekliğini ayarlar veya alır |
| [MoveTo](./moveto/) | Geçerli aralığı hedef aralığa taşı. |
| [CopyData](./copydata/) | Kaynak bir aralıktan hücre verilerini (formüller dahil) kopyalar. |
| [CopyValue](./copyvalue/) | Kaynak bir aralıktan hücre değerini kopyalar. |
| [CopyStyle](./copystyle/) | Kaynak bir aralıktan stil ayarlarını kopyalar. |
| [Copy_Range_PasteOptions](./copy_range_pasteoptions/) | Aralığı yapıştırma özel seçenekleriyle kopyalıyor. |
| [Transpose](./transpose/) | Verileri satırlardan sütunlara veya tersine (döndürerek) aktarır. |
| [Copy_Range](./copy_range/) | Kaynak bir aralıktan veri (formüller dahil), biçimlendirme, çizim nesneleri vb. kopyalar. |
| [Get](./get/) | Bu aralıktaki Cell nesnesini alır. |
| [GetCellOrNull](./getcellornull/) | Bu aralıktaki Cell nesnesini veya null değerini alır. |
| [GetOffset](./getoffset/) | Ofset ile Range aralığını alır. |
| [GetEntireColumn](./getentirecolumn/) | Belirtilen aralığı içeren tüm sütunu (veya sütunları) temsil eden bir Range nesnesi alır. |
| [GetEntireRow](./getentirerow/) | Belirtilen aralığı içeren tüm satırı (veya satırları) temsil eden bir Range nesnesi alır. |
| [GetWorksheet](./getworksheet/) | Bu aralığı içeren Worksheetobject nesnesini alır. |
| [ToString](./tostring/) | Geçerli Range nesnesini temsil eden bir dize döndürür. |
| [ToImage](./toimage/) | Aralığı görüntüye dönüştürür. |
| [ToJson](./tojson/) | Aralığı JSON değerine dönüştürür. |
| [ToHtml](./tohtml/) | Aralığı html'ye dönüştürür. |
| [Clear](./clear/) | Bu aralığı temizler. |
| [ClearContents](./clearcontents/) | Bu aralığın içeriğini temizler. |
| [ClearFormats](./clearformats/) | Bu aralığın biçimlerini temizler. |
| [ClearComments](./clearcomments/) | Bu aralığın yorumlarını temizler. |
| [ClearHyperlinks](./clearhyperlinks/) | Yalnızca köprüleri kaldırır. |
