---
title: "ReConnectionMethodType Enum"
linktitle: "ReConnectionMethodType"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "ReConnectionMethodType enum. Go dilinde reconnectionmethodtype'i temsil eden nesneyi kapsül eder."
type: docs
weight: 200
url: /tr/go-cpp/reconnectionmethodtype/
---

## ReConnectionMethodType Enum

Bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir.

```go

type ReConnectionMethodType int32


```

## Alanlar

| Alan | Açıklama |
| --- | --- |
| [Required](./required/) | Yenilemede mevcut bağlantı bilgilerini kullan ve eğer geçersiz olursa, dış bağlantı dosyasından mevcutsa güncellenmiş bağlantı bilgilerini al. |
| [Always](./always/) | Her yenilemede dış bağlantı dosyasından (varsa) güncellenmiş bağlantı bilgilerini al ve mevcut bağlantı bilgileri yerine kullan. Bu durumda dış bağlantı dosyası mevcut değilse veri yenilemesi başarısız olur. |
| [Never](./never/) | Dış bağlantı dosyasından (varsa) güncellenmiş bağlantı bilgilerini asla almaz, hatta mevcut bağlantı bilgileri geçersiz olsa bile. |
