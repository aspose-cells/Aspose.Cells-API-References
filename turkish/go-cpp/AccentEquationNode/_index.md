---
title: "AccentEquationNode Sınıfı"
linktitle: "AccentEquationNode"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "AccentEquationNode sınıfı. Go'da accentequationnode'u temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/accentequationnode/
---

## AccentEquationNode class

Bu sınıf, bir temel bileşen ve birleştirici bir diakritik içeren aksan denklemini tanımlar.

```go

type AccentEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewAccentEquationNode](./newaccentequationnode/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetAccentCharacter](./getaccentcharacter/) | Bu öznitelik, aksan işlevinin temeline eklenen birleştirici diakritik işaretin türünü belirtir. Varsayılan aksan karakteri U+0302'dir. Aksan karakterini ayarlamak için AccentType özniteliğini kullanmanız şiddetle tavsiye edilir. Bilinen bir türde ihtiyacınız olan karakteri bulamıyorsanız bu özellik ayarını kullanın. |
| [SetAccentCharacter](./setaccentcharacter/) | Bu öznitelik, aksan işlevinin temeline eklenen birleştirici diakritik işaretin türünü belirtir. Varsayılan aksan karakteri U+0302'dir. Aksan karakterini ayarlamak için AccentType özniteliğini kullanmanız şiddetle tavsiye edilir. Bilinen bir türde ihtiyacınız olan karakteri bulamıyorsanız bu özellik ayarını kullanın. |
| [GetAccentCharacterType](./getaccentcharactertype/) | Birleştirici karakterleri tür değerine göre belirtin. |
| [SetAccentCharacterType](./setaccentcharactertype/) | Birleştirici karakterleri tür değerine göre belirtin. |
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
| [AccentEquationNode_CreateNode](./accentequationnode_createnode/) | Belirtilen tipte bir düğüm oluştur. |
