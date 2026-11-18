---
title: "TxtValueQuoteType Enum"
linktitle: "TxtValueQuoteType"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "TxtValueQuoteType enum. Go'da txtvaluequotetype'ı temsil eden nesneyi kapsar."
type: docs
weight: 200
url: /tr/go-cpp/txtvaluequotetype/
---

## TxtValueQuoteType Enum

Metin biçimindeki dosyalarda değerler için tırnak işareti kullanım türünü belirtir.

```go

type TxtValueQuoteType int32


```

## Alanlar

| Alan | Açıklama |
| --- | --- |
| [Normal](./normal/) | Tırnak işareti, ayırıcı karakter gibi özel karakterler içeren tüm değerler tırnak içine alınır. Metin dosyası dışa aktarırken ms excel'in davranışıyla aynı. |
| [Always](./always/) | Tüm değerler her zaman tırnak içine alınır. |
| [Minimum](./minimum/) | Değerleri yalnızca gerektiğinde tırnak içine alın. Örneğin, bir değer tırnak işareti içeriyorsa ancak tırnak işareti bu değerin başında değilse, bu değer tırnak içine alınmayacaktır. |
| [Never](./never/) | Tüm değerler tırnak içine alınmayacaktır. Bu türde dışa aktarılan metin dosyası, gerekli tırnak işaretleri eksik olduğu için doğru şekilde geri okunamayabilir. |
