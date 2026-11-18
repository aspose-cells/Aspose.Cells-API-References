---
title: "GroupCharacterEquationNode Sınıfı"
linktitle: "GroupCharacterEquationNode"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "GroupCharacterEquationNode sınıfı. Go'da groupcharacterequationnode'u temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/groupcharacterequationnode/
---

## GroupCharacterEquationNode class

Bu sınıf, metnin üstüne veya altına çizilen bir karakterden oluşan Grup-Karakter işlevini belirtir, genellikle öğeleri görsel olarak gruplamak amacıyla.

```go

type GroupCharacterEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewGroupCharacterEquationNode](./newgroupcharacterequationnode/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetGroupChr](./getgroupchr/) | Bir sembol (varsayılan U+23DF) belirtir. Aksan karakterini ayarlamak için ChrType özniteliğini kullanmanız şiddetle önerilir. Bilinen bir türde ihtiyacınız olan karakteri bulamıyorsanız bu özellik ayarını kullanın. |
| [SetGroupChr](./setgroupchr/) | Bir sembol (varsayılan U+23DF) belirtir. Aksan karakterini ayarlamak için ChrType özniteliğini kullanmanız şiddetle önerilir. Bilinen bir türde ihtiyacınız olan karakteri bulamıyorsanız bu özellik ayarını kullanın. |
| [GetChrType](./getchrtype/) | Birleştirici karakterleri tür değerine göre belirtin. |
| [SetChrType](./setchrtype/) | Birleştirici karakterleri tür değerine göre belirtin. |
| [GetPosition](./getposition/) | Bu öznitelik, karakterin nesnedeki konumunu belirtir |
| [SetPosition](./setposition/) | Bu öznitelik, karakterin nesnedeki konumunu belirtir |
| [GetVertJc](./getvertjc/) | Bu öznitelik, groupChrPr'nin pos özelliğiyle birleştirildiğinde, groupChr nesnesinin dikey düzenini belirtir. Burada pos, gruplayıcı karakterin konumunu, vertJc ise nesnenin taban çizgisine göre hizalamasını belirtir. |
| [SetVertJc](./setvertjc/) | Bu öznitelik, groupChrPr'nin pos özelliğiyle birleştirildiğinde, groupChr nesnesinin dikey düzenini belirtir. Burada pos, gruplayıcı karakterin konumunu, vertJc ise nesnenin taban çizgisine göre hizalamasını belirtir. |
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
| [GroupCharacterEquationNode_CreateNode](./groupcharacterequationnode_createnode/) | Belirtilen tipte bir düğüm oluştur. |
