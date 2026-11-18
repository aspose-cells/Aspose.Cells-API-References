---
title: "DelimiterEquationNode Sınıfı"
linktitle: "DelimiterEquationNode"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "DelimiterEquationNode sınıfı. Go'da delimiterequationnode'ı temsil eden nesneyi kapsar."
type: docs
weight: 200
url: /tr/go-cpp/delimiterequationnode/
---

## DelimiterEquationNode class

Bu sınıf, açılış ve kapanış sınırlayıcılarından (parantez, süslü parantez, köşeli parantez ve dikey çubuk gibi) ve içinde bulunan bir bileşenden oluşan sınırlayıcı denklemini belirtir.Sınırlayıcı, her bileşen arasında belirlenmiş bir ayırıcı karakterle birden fazla bileşene sahip olabilir.

```go

type DelimiterEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewDelimiterEquationNode](./newdelimiterequationnode/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetBeginChar](./getbeginchar/) | Ayırıcı başlangıç karakteri. |
| [SetBeginChar](./setbeginchar/) | Ayırıcı başlangıç karakteri. |
| [GetEndChar](./getendchar/) | Ayırıcı bitiş karakteri. |
| [SetEndChar](./setendchar/) | Ayırıcı bitiş karakteri. |
| [GetNaryGrow](./getnarygrow/) | Ayırıcı, formül yüksekliğiyle otomatik olarak genişleyip daralması gerekip gerekmediğini belirtir. |
| [SetNaryGrow](./setnarygrow/) | Ayırıcı, formül yüksekliğiyle otomatik olarak genişleyip daralması gerekip gerekmediğini belirtir. |
| [GetSeparatorChar](./getseparatorchar/) | Ayırıcı ayırıcı karakteri. |
| [SetSeparatorChar](./setseparatorchar/) | Ayırıcı ayırıcı karakteri. |
| [GetDelimiterShape](./getdelimitershape/) | Ayırıcı nesnesindeki ayırıcıların şeklini belirtir. |
| [SetDelimiterShape](./setdelimitershape/) | Ayırıcı nesnesindeki ayırıcıların şeklini belirtir. |
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
| [DelimiterEquationNode_CreateNode](./delimiterequationnode_createnode/) | Belirtilen tipte bir düğüm oluştur. |
