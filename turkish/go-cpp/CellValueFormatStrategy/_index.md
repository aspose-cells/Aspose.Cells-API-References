---
title: "CellValueFormatStrategy Enum"
linktitle: "CellValueFormatStrategy"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "CellValueFormatStrategy enum. Go dilinde cellvalueformatstrategy nesnesini temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/cellvalueformatstrategy/
---

## CellValueFormatStrategy Enum

Hücre değerine stilin nasıl uygulanacağını belirtir.

```go

type CellValueFormatStrategy int32


```

## Alanlar

| Alan | Açıklama |
| --- | --- |
| [None](./none/) | Biçimlendirilmemiş. |
| [CellStyle](./cellstyle/) | Yalnızca hücrenin orijinal stiliyle biçimlendirilir. |
| [DisplayStyle](./displaystyle/) | Hücrenin görüntülenen stiliyle biçimlendirilir. |
| [DisplayString](./displaystring/) | MS Excel'de gösterilen görüntülenen dizeyi alır. <see cref="DisplayStyle"/> ile olan temel fark, bu seçeneğin ayrıca sütun genişliğinin etkisini de dikkate almasıdır. Sütun genişliği biçimlendirilmiş dizeyi tamamen gösterecek kadar küçükse, MS Excel'in yaptığı gibi "#" gösterilebilir. |
