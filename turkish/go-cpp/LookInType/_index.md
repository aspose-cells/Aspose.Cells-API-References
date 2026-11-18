---
title: "LookInType Enum"
linktitle: "LookInType"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "LookInType enum. Go'da lookintype'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/lookintype/
---

## LookInType Enum

İçine bakma türünü temsil eder.

```go

type LookInType int32


```

## Alanlar

| Alan | Açıklama |
| --- | --- |
| [Formulas](./formulas/) | Hücre formül ise, aranan nesneyi formülden (<see cref=\"Cell.Formula\"/>) bulur, aksi takdirde hücrenin orijinal değerinden (aynı <see cref=\"OriginalValues\"/> ile) bulur. |
| [Values](./values/) | Nesneyi hücrenin orijinal değerinden (<see cref=\"Cell.Value\"/>) ve biçimlendirilmiş değerinden (<see cref=\"Cell.StringValue\"/>) bulur. |
| [ValuesExcludeFormulaCell](./valuesexcludeformulacell/) | Formül olan hücreleri yok sayar. Formül olmayan hücreler için, <see cref=\"Values\"/> ile aynı davranır. |
| [Comments](./comments/) | Yalnızca hücrenin yorumundan nesneyi bulur. Yorumu olmayan hücreleri yok sayar. |
| [OnlyFormulas](./onlyformulas/) | Formül olmayan hücreleri yok sayar. Formül olan hücreler için, aranan nesneyi formülden (<see cref=\"Cell.Formula\"/>) bulur. |
| [OriginalValues](./originalvalues/) | Yalnızca hücrenin orijinal değerinden nesneyi bul. |
| [FormattedValues](./formattedvalues/) | Yalnızca hücrenin biçimlendirilmiş değerinden (<see cref=\"Cell.StringValue\"/>) nesneyi bul. |
