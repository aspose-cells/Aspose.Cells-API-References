---
title: "EquationNodeParagraph Sınıfı"
linktitle: "EquationNodeParagraph"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "EquationNodeParagraph sınıfı. Go dilinde equationnodeparagraph nesnesini temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/equationnodeparagraph/
---

## EquationNodeParagraph class

Bu sınıf, bir veya daha fazla MathEquationNode(OMath) öğesi içeren matematiksel bir paragrafı belirtir.

```go

type EquationNodeParagraph struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewEquationNodeParagraph](./newequationnodeparagraph/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetJustification](./getjustification/) | Bu, matematik paragrafının hizalamasını belirtir (aynı paragrafta yan yana bulunan bir dizi denklem). Bir matematik paragrafı Sol Hizalı, Sağ Hizalı, Ortalanmış veya Grup Olarak Ortalanmış olabilir. Varsayılan olarak, matematik paragrafı Grup Olarak Ortalanmıştır. Bu, denklemlerin birbirlerine göre hizalanabileceği, ancak tüm denklem grubunun bütün olarak ortalandığı anlamına gelir. |
| [SetJustification](./setjustification/) | Bu, matematik paragrafının hizalamasını belirtir (aynı paragrafta yan yana bulunan bir dizi denklem). Bir matematik paragrafı Sol Hizalı, Sağ Hizalı, Ortalanmış veya Grup Olarak Ortalanmış olabilir. Varsayılan olarak, matematik paragrafı Grup Olarak Ortalanmıştır. Bu, denklemlerin birbirlerine göre hizalanabileceği, ancak tüm denklem grubunun bütün olarak ortalandığı anlamına gelir. |
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
| [EquationNodeParagraph_CreateNode](./equationnodeparagraph_createnode/) | Belirtilen tipte bir düğüm oluştur. |
