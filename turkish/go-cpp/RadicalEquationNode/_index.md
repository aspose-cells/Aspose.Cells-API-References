---
title: "RadicalEquationNode sınıfı"
linktitle: "RadicalEquationNode"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "RadicalEquationNode sınıfı. Go'da radicalequationnode'u temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/radicalequationnode/
---

## RadicalEquationNode class

Bu sınıf, isteğe bağlı bir derece deg(EquationNodeType.Degree) ve bir tabandan oluşan radikal denklemini belirtir.

```go

type RadicalEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewRadicalEquationNode](./newradicalequationnode/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [IsDegHide](./isdeghide/) | Radikallerin derecesini gizleyip gizlemeyeceği. |
| [SetIsDegHide](./setisdeghide/) | Radikallerin derecesini gizleyip gizlemeyeceği. |
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
| [RadicalEquationNode_CreateNode](./radicalequationnode_createnode/) | Belirtilen tipte bir düğüm oluştur. |
