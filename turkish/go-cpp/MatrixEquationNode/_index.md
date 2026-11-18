---
title: "MatrixEquationNode Sınıfı"
linktitle: "MatrixEquationNode"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "MatrixEquationNode sınıfı. Go'da matrixequationnode'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/matrixequationnode/
---

## MatrixEquationNode class

Bu sınıf, bir veya daha fazla satır ve bir veya daha fazla sütunda düzenlenen bir veya daha fazla öğeden oluşan Matris denklemini belirtir.

```go

type MatrixEquationNode struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewMatrixEquationNode](./newmatrixequationnode/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetBaseJc](./getbasejc/) | Bu öznitelik matrisin hizalamasını belirtir. Matrisin dışındaki metin, matris işlevinin altına, üstüne veya ortasına hizalanabilir. Varsayılan olarak, matris orta hizalama varsayar. |
| [SetBaseJc](./setbasejc/) | Bu öznitelik matrisin hizalamasını belirtir. Matrisin dışındaki metin, matris işlevinin altına, üstüne veya ortasına hizalanabilir. Varsayılan olarak, matris orta hizalama varsayar. |
| [IsHidePlaceholder](./ishideplaceholder/) | Bu öznitelik bir matriste Gizli Yer Tutucular özelliğini belirtir. Bu özellik etkin olduğunda, yer tutucular matris içinde görünmez. Varsayılan olarak, yer tutucular görünür, böylece metnin eklenebileceği konumlar belirginleşir. |
| [SetIsHidePlaceholder](./setishideplaceholder/) | Bu öznitelik bir matriste Gizli Yer Tutucular özelliğini belirtir. Bu özellik etkin olduğunda, yer tutucular matris içinde görünmez. Varsayılan olarak, yer tutucular görünür, böylece metnin eklenebileceği konumlar belirginleşir. |
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
| [MatrixEquationNode_CreateNode](./matrixequationnode_createnode/) | Belirtilen tipte bir düğüm oluştur. |
