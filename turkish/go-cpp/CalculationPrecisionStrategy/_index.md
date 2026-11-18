---
title: "CalculationPrecisionStrategy Enum"
linktitle: "CalculationPrecisionStrategy"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "CalculationPrecisionStrategy enum. Go dilinde calculationprecisionstrategy nesnesini temsil eden nesneyi kapsar."
type: docs
weight: 200
url: /tr/go-cpp/calculationprecisionstrategy/
---

## CalculationPrecisionStrategy Enum

Hesaplama hassasiyetini ele alma stratejilerini sıralar. IEEE 754 Kayan Nokta Aritmetiği'nin hassasiyet sorunu nedeniyle, bazı "seemingly simple" formüller beklenen sonuç olarak hesaplanmayabilir. Örneğin formül "=-0.45+0.43+0.02", operantları '+' operatörüyle doğrudan hesapladığınızda sonuç sıfır olmaz. Bu tür hassasiyet sorunları için, bazı özel stratejiler beklenen sonucu verebilir.

```go

type CalculationPrecisionStrategy int32


```

## Alanlar

| Alan | Açıklama |
| --- | --- |
| [None](./none/) | Hesaplamada strateji uygulanmaz.Hesaplama yaparken sadece orijinal çift değerini operand olarak kullanın ve sonucu doğrudan döndürün.En verimli performans için ve çoğu durumda uygulanabilir. |
| [Round](./round/) | Hesaplama sonucunu anlamlı basamaklara göre yuvarlar. |
| [Decimal](./decimal/) | Mümkün olduğunda ondalık sayıları operand olarak kullanır.Performans açısından en verimsiz. |
