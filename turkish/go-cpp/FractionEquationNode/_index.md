---
title: "FractionEquationNode Sınıf"
linktitle: "FractionEquationNode"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "FractionEquationNode sınıf. Go'da fractionequationnode'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/fractionequationnode/
---

## FractionEquationNode class

Bu sınıf  kesir denklemini belirtir, bir pay ve bir payda kesir çubuğu ile ayrılmıştır. Kesir çubuğu, kesir özelliklerine bağlı olarak yatay veya diyagonal olabilir. Kesir denklemi ayrıca, bir öğeyi diğerinin üzerine yerleştiren ve kesir çubuğu olmayan yığın işlevini temsil etmek için de kullanılır.

```go

type FractionEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewFractionEquationNode](./newfractionequationnode/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetFractionType](./getfractiontype/) | Bu, kesir tipini belirtir; varsayılan 'Bar' dır. |
| [SetFractionType](./setfractiontype/) | Bu, kesir tipini belirtir; varsayılan 'Bar' dır. |
| [Equals](./equals/) | Mevcut denklem düğümünün belirtilen düğüme eşit olup olmadığını belirle |
| [GetStartIndex](./getstartindex/) | Karakterlerin başlangıç indeksini alır. |
| [GetLength](./getlength/) | Karakterlerin uzunluğunu alır. |
| [GetFont](./getfont/) | Bu nesnenin yazı tipini döndürür. |
| [SetWordArtStyle](./setwordartstyle/) | Önceden ayarlanmış WordArt stilini ayarlar. |
| [GetTextOptions](./gettextoptions/) | Metin seçeneklerini döndürür. |
| [GetType](./gettype/) | Metin düğümünün tipini alır. |
| [GetParentNode](./getparentnode/) | Geçerli düğümün üst düğümünü belirtir |
| [SetParentNode](./setparentnode/) | Geçerli düğümün üst düğümünü belirtir |
| [ToLaTeX](./tolatex/) | Bu denklemi LaTeX ifadesine dönüştür. |
| [ToMathML](./tomathml/) | Bu denklemi MathML ifadesine dönüştür. |
| [AddChild_EquationNodeType](./addchild_equationnodetype/) | Belirtilen türde bir düğümü mevcut düğümün alt düğüm listesinde sonuna ekle. |
| [InsertChild](./insertchild/) | Belirtilen türde bir düğümü mevcut düğümün alt düğüm listesinde belirtilen indeks konumuna ekler. |
| [InsertAfter](./insertafter/) | Belirtilen düğümü mevcut düğümün sonrasına ekler. |
| [InsertBefore](./insertbefore/) | Belirtilen düğümü mevcut düğümün öncesine ekler. |
| [GetChild](./getchild/) | Mevcut düğümün çocukları arasında belirtilen indeksdeki düğümü döndürür. |
| [Remove](./remove/) | Kendisini üst düğümden kaldırır. |
| [RemoveChild_EquationNode](./removechild_equationnode/) | Belirtilen düğümü mevcut düğümün çocuklarından kaldırır. |
| [RemoveAllChildren](./removeallchildren/) | Mevcut düğümün tüm alt düğümlerini kaldırır. |
| [GetEquationType](./getequationtype/) | Mevcut düğümün denklem tipini al |
| [FractionEquationNode_CreateNode](./fractionequationnode_createnode/) | Belirtilen tipte bir düğüm oluştur. |
