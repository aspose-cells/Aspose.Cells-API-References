---
title: "NaryEquationNode Sınıfı"
linktitle: "NaryEquationNode"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "NaryEquationNode sınıfı. Go'da naryequationnode'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/naryequationnode/
---

## NaryEquationNode class

Bu sınıf, bir n-ary operatör, bir taban (veya operand) ve isteğe bağlı üst ve alt sınırları içeren n-ary operatör denklemini belirtir.

```go

type NaryEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewNaryEquationNode](./newnaryequationnode/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [IsHideSubscript](./ishidesubscript/) | Alt sınırın gösterilip gösterilmeyeceği |
| [SetIsHideSubscript](./setishidesubscript/) | Alt sınırın gösterilip gösterilmeyeceği |
| [IsHideSuperscript](./ishidesuperscript/) | Üst sınırın gösterilip gösterilmeyeceği |
| [SetIsHideSuperscript](./setishidesuperscript/) | Üst sınırın gösterilip gösterilmeyeceği |
| [GetLimitLocation](./getlimitlocation/) | Bu öznitelik, n-ary operatörlerde limitlerin konumunu belirler. Limitler, n-ary operatörün üstünde ve altında ortalanmış ya da operatörün hemen sağında konumlandırılmış olabilir. |
| [SetLimitLocation](./setlimitlocation/) | Bu öznitelik, n-ary operatörlerde limitlerin konumunu belirler. Limitler, n-ary operatörün üstünde ve altında ortalanmış ya da operatörün hemen sağında konumlandırılmış olabilir. |
| [GetNaryOperator](./getnaryoperator/) | bir n-ary operatör. örn. "∑". n-ary operatörü ayarlamak için NaryOperatorType özniteliğini kullanmanız şiddetle tavsiye edilir. Bilinen bir türde ihtiyacınız olan karakteri bulamıyorsanız bu özellik ayarını kullanın. |
| [SetNaryOperator](./setnaryoperator/) | bir n-ary operatör. örn. "∑". n-ary operatörü ayarlamak için NaryOperatorType özniteliğini kullanmanız şiddetle tavsiye edilir. Bilinen bir türde ihtiyacınız olan karakteri bulamıyorsanız bu özellik ayarını kullanın. |
| [GetNaryOperatorType](./getnaryoperatortype/) | bir n-ary operatör. örn. "∑" |
| [SetNaryOperatorType](./setnaryoperatortype/) | bir n-ary operatör. örn. "∑" |
| [GetNaryGrow](./getnarygrow/) | Bu öznitelik, belge seviyesinde n-ary operatörlerin büyüme özelliğini belirler. Kapalı olduğunda, integraller ve toplamlar gibi n-ary operatörler, işlenenin yüksekliğine göre büyümez. Açık olduğunda, n-ary operatör dikey olarak işlenenin yüksekliğine uyacak şekilde büyür. |
| [SetNaryGrow](./setnarygrow/) | Bu öznitelik, belge seviyesinde n-ary operatörlerin büyüme özelliğini belirler. Kapalı olduğunda, integraller ve toplamlar gibi n-ary operatörler, işlenenin yüksekliğine göre büyümez. Açık olduğunda, n-ary operatör dikey olarak işlenenin yüksekliğine uyacak şekilde büyür. |
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
| [NaryEquationNode_CreateNode](./naryequationnode_createnode/) | Belirtilen tipte bir düğüm oluştur. |
