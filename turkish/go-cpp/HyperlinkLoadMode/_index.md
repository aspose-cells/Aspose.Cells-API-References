---
title: "HyperlinkLoadMode Enum"
linktitle: "HyperlinkLoadMode"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "HyperlinkLoadMode enum. Go dilinde hyperlinkloadmode nesnesini temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/hyperlinkloadmode/
---

## HyperlinkLoadMode Enum

HTML yüklenirken köprülerin nasıl işlendiğini belirtir.

```go

type HyperlinkLoadMode int32


```

## Alanlar

| Alan | Açıklama |
| --- | --- |
| [Normal](./normal/) | Bir hücrede yalnızca ilk köprü yüklenir, sonraki köprüler göz ardı edilir. |
| [AllowMultiple](./allowmultiple/) | Bir hücredeki tüm köprüler <see cref="Worksheet.Hyperlinks"/> öğesine eklenir. MS Excel'in kendisinin bir hücrede yalnızca bir köprüyi desteklediğini unutmayın, bu nedenle bu seçenek Excel'in tam olarak görüntüleyemediği dosyalar üretebilir. |
