---
title: "EquationNodeType Enum"
linktitle: "EquationNodeType"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "EquationNodeType enum. Go dilinde equationnodetype'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/equationnodetype/
---

## EquationNodeType Enum

Denklik düğüm tipi. Not:(1)[1-99] Şu anda kapsamda yalnızca bir düğüm var ve onun sayı değeri 1'dir. Belirttiği düğüm matematiksel metni depolamak için kullanılır. (2)[100-199] Düğümün bazı özel fonksiyon düğümlerinin bir bileşeni olduğunu gösterir. (3)[200-] Düğümün bazı özel işlevlere sahip olduğunu gösterir.

```go

type EquationNodeType int32


```

## Alanlar

| Alan | Açıklama |
| --- | --- |
| [UnKnow](./unknow/) | UnKnow |
| [Text](./text/) | matematik metnini depolayan bir düğüm belirtir |
| [Base](./base/) | Bir Base bileşeni belirtir |
| [Denominator](./denominator/) | Bir Denominator bileşeni belirtir |
| [Numerator](./numerator/) | Bir Numerator bileşeni belirtir |
| [FunctionName](./functionname/) | Bir FunctionName bileşeni belirtir |
| [Subscript](./subscript/) | Bir Subscript bileşeni belirtir |
| [Superscript](./superscript/) | Bir Superscript bileşeni belirtir |
| [Degree](./degree/) | Bir Degree bileşeni belirtir |
| [MatrixRow](./matrixrow/) | Bir MatrixRow bileşeni belirtir. Matrisin tek bir satırı |
| [Limit](./limit/) | Lower-Limit işlevi veya Upper-Limit işlevinin bir alt nesnesini temsil eder |
| [EquationParagraph](./equationparagraph/) | Bir matematik paragrafı (oMathPara) belirtir. |
| [LowerLimit](./lowerlimit/) | Lower-Limit işlevini belirtir |
| [UpperLimit](./upperlimit/) | Upper-Limit işlevini belirtir |
| [Mathematical](./mathematical/) | Bir denklem veya matematiksel ifade (OMath) belirtir. |
| [Fraction](./fraction/) | Kesirli denklemi belirtir |
| [Function](./function/) | Fonksiyon denklemini belirtir |
| [Delimiter](./delimiter/) | Ayırıcı denklemi belirtir |
| [Nary](./nary/) | n-ary operatör denklemini belirtir |
| [Radical](./radical/) | Kök denklemini belirtir |
| [Sup](./sup/) | Üst simge denklemini belirtir |
| [Sub](./sub/) | Alt simge denklemini belirtir |
| [SubSup](./subsup/) | İşleçlerin sağında üst ve alt simgelerle bir denklemi belirtir. |
| [PreSubSup](./presubsup/) | İşleçlerin solunda üst ve alt simgelerle bir denklemi belirtir. |
| [Accent](./accent/) | Aksan denklemini belirtir |
| [Bar](./bar/) | Bar denklemini belirtir |
| [BorderBox](./borderbox/) | Kenarlık kutusu denklemini belirtir |
| [Box](./box/) | Kutu denklemini belirtir |
| [GroupChr](./groupchr/) | Grup karakter denklemini belirtir |
| [Matrix](./matrix/) | Matris denklemini belirtir, |
| [ArrayEquation](./arrayequation/) | Denklem-Dizisi işlevini belirtir. İşlev bir veya daha fazla denklemden oluşur. |
